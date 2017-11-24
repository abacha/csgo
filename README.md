//Guns & Grenades
bind "F" 							"slot7"			//FLASHBANG
bind "Q" 							"slot10" 		//MOLOTOV
bind "MOUSE3" 						"slot8" 		//SMOKE
bind "MWHEELUP" 					"slot1"
bind "MWHEELDOWN" 					"slot3"

//Movement
bind "MOUSE1" 						"+attack"
bind "MOUSE2" 						"+jump"
bind "MOUSE5" 						"+attack2"
bind "SPACE" 						"+duck"
bind "V" 							"+jumpthrow"

//Game Play
bind "ctrl" 						"lastinv"
bind "MOUSE4" 						"+voicerecord"
bind "TAB" 							"+showscores"
bind "capslock" 					"+lookatweapon"

alias +jumpthrow "+jump; -attack"
alias -jumpthrow "-jump"

// Crosshair
crosshair 							"1" 			//Enables crosshair
cl_crosshairstyle 					"4" 			//Enter this first to customize a crosshair that is static.

cl_crosshairusealpha 				"1" 			//Allows the crosshair to be solid
cl_crosshairalpha 					"255" 			//Keeps the color solid, not see through
cl_crosshaircolor 					"1" 			//Allows custom colors.
cl_crosshaircolor_b 				"255" 			//Blue
cl_crosshaircolor_g 				"255"		 	//Green
cl_crosshaircolor_r 				"255" 			//Red
cl_crosshairdot						"0" 			//Dot in the center off, +1 if you want it on
cl_crosshairgap 					"-2" 			//Gap in the middle of the cross
cl_crosshairsize 					"3" 			//Size of the cross
cl_crosshairthickness 				"0.6" 			//Thickness of the cross
cl_crosshair_drawoutline			"1" 			//Increases visibility on white crosshairs
cl_crosshair_outlinethickness 		"1" 			//Thickness of the outline

//Buy Binds
bind "kp_uparrow" 					"buy ump45;"
bind "kp_ins" 						"buy vest; buy vesthelm;"
bind "kp_5" 						"buy smokegrenade;"
bind "kp_end" 						"buy galilar; buy famas;"
bind "kp_downarrow" 				"buy ak47; buy m4a1;"
bind "kp_pgdn" 						"buy flashbang;"
bind "kp_leftarrow" 				"buy hegrenade;"
bind "kp_rightarrow" 				"buy molotov; buy incgrenade;"
bind "kp_del" 						"buy p250;"
bind "kp_home" 						"buy tec9; buy fiveseven;"
bind "kp_pgup" 						"buy awp;"
bind "kp_multiply" 					"buy defuser"
bind "kp_slash" 					"buy mac10; buy mp9"

echo "+=====================================================+"
echo "|     NUM     |      /      |      *      |     -     |"
echo "|     PAD     | MAC-10/MP9  |    DEFUSE   |   DEAGLE  |"
echo "|-------------|-------------|-------------|-----------|"
echo "|      7      |      8      |      9      |     +     |"
echo "|    TEC-9    |   UMP-45    |     AWP     |           |"
echo "|-------------|-------------|-------------|           |"
echo "|      4      |      5      |      6      |           |"
echo "|     HE      |    SMOKE    |   MOLOTOV   |           |"
echo "|-------------|-------------|-------------|-----------|"
echo "|      1      |      2      |      3      |   ENTER   |"
echo "| FAMAS/GALIL |   AK/COLT   |    FLASH    |           |"
echo "|-------------|-------------|-------------|           |"
echo "|             0             |      .      |           |"
echo "|         KEV+HELMET        |    p250     |           |"
echo "+=====================================================+"


//Mouse 
m_rawinput 							"1"
m_mouseaccel1 						"0"
m_mouseaccel2 						"0"
m_mousespeed 						"0"
zoom_sensitivity_ratio_mouse		"0.9"
sensitivity 						"0.9"


// Net Graph
net_graph 							"1"
net_graphpos 						"1"
net_graphheight 					"0"
net_graphproportionalfont 			"1"


//Radar
cl_radar_always_centered 			"0"
cl_radar_icon_scale_min				"0.4"
cl_radar_rotate						"1"
cl_radar_scale 						"0.5"
hud_scaling 						"0.88"

alias "+radar" "cl_radar_scale 0.2"
alias "-radar" "cl_radar_scale 0.4"


//Rates and Interpolation
net_graph 							"0"
net_graphpos 						"1"
net_graphheight 					"0"
rate 								"786432"
cl_cmdrate 							"128"
cl_updaterate 						"128"
cl_interp 							"0"
cl_interp_ratio 					"1"

//Viewmodel
cl_righthand 						"0"
cl_color							"2"
cl_showhelp 						"0" 
cl_autowepswitch 					"0"

//Sounds
snd_deathcamera_volume 				"0"
snd_mapobjective_volume				"0"
snd_menumusic_volume 				"0"
snd_musicvolume 					"0.5"
snd_roundstart_volume 				"0"
snd_roundend_volume 				"0"
snd_tensecondwarning_volume 		"0.1"
snd_use_hrtf 						"1"
windows_speaker_config				"1"
volume								"0.3"
voice_scale							"0.3"
voice_enable						"1"
snd_mute_losefocus 					"0"


host_writeconfig

//-console -novid -freq 144 -noaafonts -nod3d9ex1 +mat_queue_mode 2 -cl_forcepreload 1 -tickrate 128 +clientport 27066 -high +exec duke.cfg

cl_autobuy vesthelm vest m4a1 ak47 famas galilar ump45
+cl_show_team_equipment
