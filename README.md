# wp-all-solutation


//  category supported portfolio

add_action('init', 'register_portfolio_type');
function register_portfolio_type() {
register_post_type('deshicoderportfolio',
		array(	'label' => 'portfolio',
				'public' => true,
				'capability_type' => 'post',
				'supports' => array('title','editor','thumbnail',),
				'taxonomies' => array('category',)
				) );
}
