how will aspect ratios be maintained with squashed or wide boxes?
  i think i'll remove short and thin boxes
    hard to make look okay on smaller screen sizes
  but keep tall and wide boxes
    but only INSIDE the regular sized boxes, not top-level
    easier to make look good on smaller screen sizes
    they can just squash down to regular boxes


use class "box" for all boxes, nested or not
  modifiers: tall/wide, bg color, text color, text alignment

use nav element for nav with links to other pagesch

don't worry about tablet viewports -- they don't matter that much