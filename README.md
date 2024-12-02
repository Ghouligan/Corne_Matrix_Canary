Simple Build using the Canary Matrix layout for the Corne Wireless Keyboard with a couple custimzed layers/mods to improve workflow. Give it a try or add on!
 
KeyMapping Below  
  
  
  
  keymap {
        compatible = "zmk,keymap";

        Canary_Matrix_layer {
            // -----------------------------------------------------------------------------------------
            // |  TAB |  Q  |  W  |  E  |  R  |  T  |   |  Y  |  U   |  I  |  O  |  P  | BKSP |
            // | CTRL |  A  |  S  |  D  |  F  |  G  |   |  H  |  J   |  K  |  L  |  ;  |  '   |
            // | SHFT |  Z  |  X  |  C  |  V  |  B  |   |  N  |  M   |  ,  |  .  |  /  | ESC  |
            //                    | GUI | LWR | SPC |   | ENT | RSE  | ALT |

            display-name = "Base";
            bindings = <
&kp TAB    &kp W  &kp L  &kp Y     &kp P  &kp B        &kp Z    &kp F  &kp O      &kp U    &kp SQT   &kp BSPC
&kp LCTRL  &kp C  &kp R  &kp S     &kp T  &kp G        &kp M    &kp N  &kp E      &kp I    &kp A     &kp SEMICOLON
&kp LSHFT  &kp Q  &kp J  &kp V     &kp D  &kp K        &kp X    &kp H  &kp COMMA  &kp DOT  &kp FSLH  &kp ESC
                         &kp LGUI  &mo 2  &kp SPACE    &kp RET  &mo 1  &kp RALT
            >;
        };

        NumPad_layer {
            // -----------------------------------------------------------------------------------------
            // |  TAB |  !  |  @  |  #  |  $  |  %  |   |  ^  |  &  |  *  |  (  |  )  | BKSP |
            // | CTRL |     |     |     |     |     |   |  -  |  =  |  [  |  ]  |  \  |  `   |
            // | SHFT |     |     |     |     |     |   |  _  |  +  |  {  |  }  | "|" |  ~   |
            //                    | GUI |     | SPC |   | ENT |     | ALT |

            display-name = "Raise";
            bindings = <
&kp TAB    &none  &htap AMPERSAND KP_NUMBER_7    &htap ASTERISK KP_NUMBER_8     &htap LEFT_PARENTHESIS KP_NUMBER_9  &none              &kp CARET   &kp LEFT_PARENTHESIS  &kp RIGHT_PARENTHESIS  &kp LESS_THAN  &kp GREATER_THAN  &kp BSPC
&kp LCTRL  &none  &htap DOLLAR KP_NUMBER_4       &htap PERCENT KP_NUMBER_5      &htap CARET KP_NUMBER_6             &kp KP_NUMBER_0    &kp LEFT    &kp UP_ARROW          &kp DOWN               &kp RIGHT      &kp MINUS         &kp GRAVE
&kp LSHFT  &none  &htap EXCLAMATION KP_NUMBER_1  &htap AT_SIGN LS(KP_NUMBER_2)  &htap HASH KP_NUMBER_3              &none              &kp K_COPY  &kp K_PASTE           &kp COMMA              &kp PERIOD     &kp SLASH         &kp ESCAPE
                                                 &kp LGUI                       &trans                              &kp SPACE          &kp RET     &trans                &kp RALT
            >;
        };

        BT-Media_layer {
            // -----------------------------------------------------------------------------------------
            // |  TAB |  1  |  2  |  3  |  4  |  5  |   |  6  |  7  |  8  |  9  |  0  | BKSP |
            // | BTCLR| BT1 | BT2 | BT3 | BT4 | BT5 |   | LFT | DWN |  UP | RGT |     |      |
            // | SHFT |     |     |     |     |     |   |     |     |     |     |     |      |
            //                    | GUI |     | SPC |   | ENT |     | ALT |

            display-name = "Lower";
            bindings = <
&kp TAB           &none         &none         &bt BT_CLR    &none         &none           &none    &none              &none            &none             &none   &kp BSPC
&kp LEFT_CONTROL  &bt BT_SEL 0  &bt BT_SEL 1  &bt BT_SEL 2  &bt BT_SEL 3  &bt BT_SEL 4    &none    &kp C_VOLUME_DOWN  &kp C_VOLUME_UP  &kp K_MUTE        &trans  &trans
&kp LSHFT         &trans        &trans        &trans        &trans        &trans          &trans   &kp K_PREVIOUS     &kp K_NEXT       &kp K_PLAY_PAUSE  &trans  &kp ESCAPE
                                              &kp LGUI      &trans        &kp SPACE       &kp RET  &trans             &kp RALT
            >;
        };
    };
};
