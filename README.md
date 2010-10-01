Another jQuery Konami Code plugin!
=================================

As the title would suggest, this is yet another konami-code jquery plugin. This one however gives you the ability to write textual key mappings.

Usage
------

If you want to use the jQuery konami plugin, then follow the next steps:

 <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.4.2/jquery.min.js" t ype="text/javascript" charset="utf-8"></script>

Then include the jquery.konami.js code like such:

 <script type="text/javascript" src="jquery.konami.js" charset="utf-8"></script>

Then in your page you'll have to add the konami handler to the body like such:

 <script type="text/javascript" charset="utf-8">
     $(document).konami({
         callback: function() {
             alert('コナミコマンド');
         }
     });
 </script>

Or you could also define your own textual or non-textual keycodes:
 <script type="text/javascript" charset="utf-8">
     $(document).konami({
         codes: ['left', 'left', 'right'],
         callback: function() {
             alert('コナミコマンド');
         }
     });
 </script>

*Beware that only 'left', 'right', 'up', 'down', 'a', 'b' are defined. If you want any other keycodes, enter them using their digit key codes as such as:

 <script type="text/javascript" charset="utf-8">
     $(document).konami({
         codes: ['left', 'left', 'right', 42, 44, 54],
         callback: function() {
             alert('コナミコマンド');
         }
     });
 </script>

Hope you enjoy!

License
-------

Simply put, New BSD.
