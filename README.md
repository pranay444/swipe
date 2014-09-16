swipe
=====
Usage
First I will show how to use the plugin. Multiple swipe events can be bound to different nodes but for the sake of example, we will use the "body".

$("body").swipe(function( direction, offset ) {
  console.log( "Moving", direction.x, "and", direction.y );
  console.log( "Touch moved by", offset.x, "horizontally and", offset.y, "vertically" );    
});


I have not released this code as an official plugin because I believe that although a good example, it serves my needs very precisely and would not be a great fit for other projects. For example, the direction argument in the callback gives "left", "right", "top" or "bottom" as values, this could be easily calculated from the secondary offset argument by checking if the values were negative or not instead.

