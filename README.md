# notificationManager
notificationManager Class

Requires jQuery

The notification manager allows you to pop notifications into view using only a few lines of js.
You can specify the container that holds the notifications when creating the class, as well as the screen position:

    var nManager = new notificationManager({container: $( '#container'), position: "topleft" });

Or define them later using: 

    nManager.setContainer( $('#container') );
    nManager.setPosition( "bottomleft" );           //String options: topleft, topright, bottomleft, bottomright

The container can be a jQuery object, or a string used in a jQuery constructor.

Next, to display a notification, use any of the following:

    nManager.addNotification(
    {
        message: "Notification message here",       //string: notification text (Html supported)
        animate: true,                              //boolean: animate the fade in as well as the progress timer/bar
        autoremove: true,                           //boolean: remove this notification from the DOM after the animation is done
        backgroundColor: "#B5D3ED",                 //string: background color of the notification
        progressColor: "#98BFE0"                    //string: color of the progress timer/bar
    });

*/
