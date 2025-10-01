■LOG
INSERT INTO operation_log VALUES (...$x)
UPDATE operation_log SET (...) VALUES (...$x)


DROP TABLE IF EXISTS operation_logs,oprations;


■CONFIG
homepage_bg_pic_url
profile_bg_pic_url
...
homepage_disc
profile_disc
work_disc
...
ui_plan
save_strategy_plan
...

■POSTS

id
title
slug
summary
markdown_body
thumbnail
genre_id
user_id
uploaded_at
modified_at
is_deleted


■DRAFTS

id
title
slug
summary
markdown_body
thumbnail
genre_id
user_id
created_at
modified_at
is_deleted


■WORK

id
name
slug
external_url
discribe


■GENRES

id
genre
slug
disc
created_at
modified_at
is_deleted

■TAGS

id
tag
slug
disc
created_at
modified_at
is_deleted


■POST_TAGS
id
post_id
tag_id
is_deleted


■admins

id
username
slug
password 	// hashed
email    	// 0auth
role
created_at
modified_at
is_deleted

■COMMENT

id
parent_id  	//nested
post_id
username
email
ip_address
published_at
is_deleted
is_censored
censored_at


■OPRATIONS

id
opration
slug
genre
is_deleted



■OPRATION_USERS

id
opration_id
admin_id
admin_ip
result_code
result_message
device
target_id
target_type
created_at
is_deleted
