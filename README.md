# Parsely API Integration Plugin

This plugin is used to show top posts, user recommendation posts, and trending tags

---

This plugin allows users to show top trending posts, show recommendation posts in a single post page and also show trending tags 

![image](https://github.com/devwingman/parsely-relevant-article-single-post/assets/170316105/4cb22179-63a0-4941-8f9e-e19249ccf34e)


---

# ⛔ Prerequisites

## 1 ACTIVE `Parsely`

Ensure Parsely is active on this site.

<aside>
⚠️ Ensure Parsely has been activated via the `vip-config.php` method.

</aside>
---

# ACTIVATE Parsely API Integration Plugin

1. ACTIVATE the Plugin
    
![image](https://github.com/devwingman/parsely-relevant-article-single-post/assets/170316105/bbe72a3b-50b8-4bcb-839e-3b99486d08d3)

    
    1. GO TO WP Admin > Plugins
    2. CLICK “Activate” next to Parsely API Integration
2. GO TO WP Admin > Parsely API Setting 
    - Screenshot
        
        ![image](https://github.com/devwingman/parsely-relevant-article-single-post/assets/170316105/90130206-c21b-44a8-a006-5d5e833c775d)

        
3. POPULATE Parsely credentials: `Parsely API key` , `Secret key`, and `Endpoint URL` . Then SAVE
    - Screenshot
        
        ![image](https://github.com/devwingman/parsely-relevant-article-single-post/assets/170316105/16f49bc4-0071-4f7b-8068-cbbda1c98a6d)

        
4. Done

# Use/Guidelines

### For showing posts and tags

1. For showing Recommendation Posts to users on a single post file use this shortcode in the sidebar
    - `<?php echo do_shortcode('[personalized_sidebar_widget]'); ?>`
    - `[personalized_sidebar_widget]`
2. For showing trending tags use this shortcode
    - `<?php echo do_shortcode('[parsely_trending_tags]'); ?>`
    - `[parsely_trending_tags]`
3. To show top trending posts use this shortcode
    - `<?php echo do_shortcode('[parsely_trending_posts offset=0 limit=3]'); ?>`
    - `[parsely_trending_posts offset=0 limit=3]`
    
    > Add `offset` and `limit` to show posts 
    Max limit is equal to `25`
    Make sure that `offset` cannot be greater then `limit`
    >
