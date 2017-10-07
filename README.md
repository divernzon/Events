# Events
Event Listing


/*** Custom Post Type ***/
function create_post_type() {

    register_post_type( 'Events',

        array(

            'labels' => array(

                'name' => __( 'Events' ),

                'singular_name' => __( 'Events' ),

                'add_new_item' => __( 'Add New Events' ),

                'edit_item' => __( 'Edit Events' ),

                'new_item' => __( 'New Events' ),

                'view_item' => __( 'View Events' ),

                'search_items' => __( 'Search Events' ),

                'not_found' => __( 'No Events found' ),

                'not_found_in_trash' => __( 'No Events found in Trash' )

            ),

            'public' => true,

            'supports' => array('title','editor','custom-fields','thumbnail')

        )

    );
}

add_action( 'init', 'create_post_type' );
/*** End of Custom Post Type ***/

This Requirements can be done by adding Advanced Custom Fields Plugin
- event date (date picker)
- event location
- URL for the event
