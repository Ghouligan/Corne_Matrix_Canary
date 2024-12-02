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

        };

        NumPad_layer {
            // -----------------------------------------------------------------------------------------
            // |  TAB |  !  |  @  |  #  |  $  |  %  |   |  ^  |  &  |  *  |  (  |  )  | BKSP |
            // | CTRL |     |     |     |     |     |   |  -  |  =  |  [  |  ]  |  \  |  `   |
            // | SHFT |     |     |     |     |     |   |  _  |  +  |  {  |  }  | "|" |  ~   |
            //                    | GUI |     | SPC |   | ENT |     | ALT |

            display-name = "Raise";


        BT-Media_layer {
            // -----------------------------------------------------------------------------------------
            // |  TAB |  1  |  2  |  3  |  4  |  5  |   |  6  |  7  |  8  |  9  |  0  | BKSP |
            // | BTCLR| BT1 | BT2 | BT3 | BT4 | BT5 |   | LFT | DWN |  UP | RGT |     |      |
            // | SHFT |     |     |     |     |     |   |     |     |     |     |     |      |
            //                    | GUI |     | SPC |   | ENT |     | ALT |

            display-name = "Lower";
