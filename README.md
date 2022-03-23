# custom-post-type-register

function Saurav_theme_custom_posts(){
                register_post_type('slide', array(
                
                    'public'      => true,
                    'label'       => 'Saurav Slider',
                    'labels'       => array(
                        
                        'name'      => 'slides',
                        'singular_name'  => 'slide',
                        'add_new'      => 'Add new Slide',
                    ),
                    'supports' => array('title', 'editor', 'thumbnail', 'excerpt')
                    
                ));
    
    
}

add_action( 'init', 'Saurav_theme_custom_posts' );
