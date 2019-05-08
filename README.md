# ![LOGO](logo.png) watchful.li **flow**ground Connector

## Description

A generated **flow**ground connector for the watchful.li API (version 1.0.0).

Generated from: https://api.apis.guru/v2/specs/watchful.li/1.0.0/swagger.json<br/>
Generated at: 2019-05-07T17:44:50+03:00

## API Description



## Authorization

This API does not require authorization.

## Actions

### Get a list of audits

> Returns a list of audits

*Tags:* `audits`

#### Input Parameters
* `limit` - _optional_ - Number of object to return (max 100, default 25)
* `limitstart` - _optional_ - Start of the return (default 0)
* `order` - _optional_ - ORDER by this field separete by comas. Add + / - after field for set ASC / DESC: type+,name-

### Get the list of fields

> Returns a list of fields

*Tags:* `audits`

### Delete a specific audit

*Tags:* `audits`

#### Input Parameters
* `id` - _required_ - ID of audit that needs to be deleted

### Find audit by ID

> Returns a audit based on ID

*Tags:* `audits`

#### Input Parameters
* `id` - _required_ - ID of audit that needs to be fetched
* `fields` - _optional_ - Fields to return separate by comas: name,id

### Get a list Extensions

> Returns a list Extensions

*Tags:* `extensions`

#### Input Parameters
* `ext_name` - _optional_ - Do a 'LIKE' search, you can also use '%'
* `siteids` - _optional_ - List of sites id separated by comma
* `ext_prefix` - _optional_ - Do a 'LIKE' search, you can also use '%'. technical name of the extension com_xxxx
* `version` - _optional_ - Do a 'LIKE' search, you can also use '%'
* `vUpdate` - _optional_ - update available for this extension
    Possible values: 1, 0.
* `fields` - _optional_ - Fields to return separate by comas: name,id
* `limit` - _optional_ - Number of object to return (max 100, default 25)
* `limitstart` - _optional_ - Start of the return (default 0)
* `order` - _optional_ - ORDER by this field separete by comas. Add + / - after field for set ASC / DESC: type+,name-

### Get the list of fields

> Returns a list of fields

*Tags:* `extensions`

### Set 'ignore updates' for a given extension / site_id

*Tags:* `extensions`

#### Input Parameters
* `id` - _required_ - ID of the extension

### Remove 'ignore updates' for a given extension

*Tags:* `extensions`

#### Input Parameters
* `id` - _required_ - ID of the extension

### Update the extension on the remote site

*Tags:* `extensions`

#### Input Parameters
* `id` - _required_ - ID of the extension

### Get feedbacks

> Returns a list of feedbacks

*Tags:* `feedbacks`

#### Input Parameters
* `fields` - _optional_ - Fields to return separate by comas (es. name,id)

### Create a feedback

*Tags:* `feedbacks`

### Get the list of fields

> Returns a list of fields

*Tags:* `feedbacks`

### Get a list of logs

> Returns a list of logs

*Tags:* `logs`

#### Input Parameters
* `log_type` - _optional_ - Type of the log
    Possible values: , plugin_sends_error, curlerror, modified_file, word_not_in_homepage, file_not_exists, update_available, new_extension, deleted_extension, extension_not_saved, modified_value_files, custom.
* `log_entry` - _optional_ - Do a 'LIKE' search, you can also use '%'
* `from` - _optional_ - Logs after this date, format YYYY-MM-DD HH:MM:SS
* `to` - _optional_ - Logs before this date, format YYYY-MM-DD HH:MM:SS
* `fields` - _optional_ - Fields to return separate by comas: name,id
* `limit` - _optional_ - Number of object to return (max 100, default 25)
* `limitstart` - _optional_ - Start of the return (default 0)
* `order` - _optional_ - ORDER by this field separete by comas. Add + / - after field for set ASC / DESC: type+,name-

### Get a CSV or PDF file contain the list of logs

> Returns a file contain the list of logs

*Tags:* `logs`

#### Input Parameters
* `format` - _required_ - Format of exported file (PDF or CSV)
    Possible values: csv, pdf.
* `site` - _optional_ - Site id of the log
* `filter_type` - _optional_ - Type of the log
    Possible values: , plugin_sends_error, curlerror, modified_file, word_not_in_homepage, file_not_exists, update_available, new_extension, deleted_extension, extension_not_saved, modified_value_files, custom.
* `search` - _optional_ - Do a 'LIKE' search, you can also use '%'
* `startdate` - _optional_ - Logs after this date, format YYYY-MM-DD HH:MM:SS
* `enddate` - _optional_ - Logs before this date, format YYYY-MM-DD HH:MM:SS
* `limit` - _optional_ - Number of object to return (max 100, default 25)
* `startid` - _optional_ - Start of the return (default 0)

### Get the list of fields

> Returns a list of fields

*Tags:* `logs`

### Get the list of log types

> Returns a list of log types

*Tags:* `logs`

### Delete a specific log

*Tags:* `logs`

#### Input Parameters
* `id` - _required_ - ID of log that needs to be deleted

### post_packages

### Returns a PDF report for a specific site

> Returns a PDF report based on a site ID

*Tags:* `reports`

#### Input Parameters
* `id` - _required_ - ID that needs to be fetched
* `from` - _optional_ - Start of the report, format YYYY-MM-DD, default today-30day 
* `to` - _optional_ - End of the report, format YYYY-MM-DD, default today
* `reports` - _optional_ - Type of reports separate by comas: Ga,Logs,Uptime
* `log_type` - _optional_ - Type of the log to show in the report
    Possible values: , plugin_sends_error, curlerror, modified_file, word_not_in_homepage, file_not_exists, update_available, new_extension, deleted_extension, extension_not_saved, modified_value_files.
* `compare` - _optional_ - Define if you want show previous values in Google Analytics graph
    Possible values: 0, 1.

### Find sites by ID

> Returns a report based on a site ID

*Tags:* `reports`

#### Input Parameters
* `id` - _required_ - ID that needs to be fetched
* `from` - _optional_ - Start of the report, format YYYY-MM-DD, default today-30day 
* `to` - _optional_ - End of the report, format YYYY-MM-DD, default today
* `reports` - _optional_ - Type of reports separate by comas: Ga,Logs,Uptime
* `log_type` - _optional_ - Type of the log to show in the report
    Possible values: , plugin_sends_error, curlerror, modified_file, word_not_in_homepage, file_not_exists, update_available, new_extension, deleted_extension, extension_not_saved, modified_value_files.
* `compare` - _optional_ - Define if you want show previous values in Google Analytics graph
    Possible values: 0, 1.

### Get a list of Sites

> Returns a list of Sites

*Tags:* `sites`

#### Input Parameters
* `siteids` - _optional_ - List of sites id separated by comma
* `name` - _optional_ - Site name. Do a 'LIKE' search, you can also use '%'
* `access_url` - _optional_ - Access URL. Do a 'LIKE' search, you can also use '%'
* `j_version` - _optional_ - Joomla version. Do a 'LIKE' search, you can also use '%'
* `ip` - _optional_ - Ip address. Do a 'LIKE' search, you can also use '%'
* `jUpdate` - _optional_ - Joomla core update status (1: update required, 0: update not required)
    Possible values: 1, 0.
* `canUpdate` - _optional_ - canUpdate
    Possible values: 1, 0.
* `published` - _optional_ - Is published
    Possible values: 1, 0.
* `error` - _optional_ - Has errors
* `nbUpdates` - _optional_
* `up` - _optional_ - Is online
    Possible values: 1, 0.
* `fields` - _optional_ - Fields to return separated by commas (e.g. name,id)
* `limit` - _optional_ - Number of objects to return (max 100, default 25)
* `limitstart` - _optional_ - Start of the return (default 0)
* `order` - _optional_ - ORDER by this field separete by comas. Add + / - after field for set ASC / DESC: type+,name-

### Create a site

*Tags:* `sites`

### Get the list of fields

> Returns a list of fields

*Tags:* `sites`

### Delete a specific Site

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of Site that needs to be deleted

### Find sites by ID

> Return a site based on ID

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID that needs to be fetched
* `fields` - _optional_ - Fields to return separate by comas: name,id

### Update a site

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website that needs to be update

### Return audits for a specific website

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website
* `fields` - _optional_ - Fields to return separate by comas: name,id
* `limit` - _optional_ - Number of object to return (max 100, default 25)
* `limitstart` - _optional_ - Start of the return (default 0)
* `order` - _optional_ - ORDER by this field

### Create an audit for the site

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website

### Add the site to the backup queue

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website

### Return backup profile

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website

### List of latest backups

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website

### Start a remote backup for the site

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website

### Step (continue) a remote backup for the site

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website

### Get extensions for a site

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website
* `fields` - _optional_ - Fields to return separate by comas: name,id
* `limit` - _optional_ - Number of object to return (max 100, default 25)
* `limitstart` - _optional_ - Start of the return (default 0)
* `order` - _optional_ - ORDER by this field

### Install extension

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website
* `url` - _required_ - URL to install the extension from

### Return logs for a specific website

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website
* `log_entry` - _optional_ - Do a 'LIKE' search, you can also use '%'
* `log_type` - _optional_ - Type of the log
    Possible values: , plugin_sends_error, curlerror, modified_file, word_not_in_homepage, file_not_exists, update_available, new_extension, deleted_extension, extension_not_saved, modified_value_files.
* `from` - _optional_ - Logs after this date, format YYYY-MM-DD HH:MM:SS
* `to` - _optional_ - Logs before this date, format YYYY-MM-DD HH:MM:SS
* `fields` - _optional_ - Fields to return separate by comas: name,id
* `limit` - _optional_ - Number of object to return (max 100, default 25)
* `limitstart` - _optional_ - Start of the return (default 0)
* `order` - _optional_ - ORDER by this field separete by comas. Add + / - after field for set ASC / DESC: type+,name-

### Create a custom log for a specific website

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website

### Delete uptime monitor

> Return boolean

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website

### Post uptime monitor

> Return boolean

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website

### Scan the site for malware

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website

### SEO analyze for a page

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website

### Return tags for a specific website

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website
* `name` - _optional_ - Do a 'LIKE' search, you can also use '%'
* `type` - _optional_ - Bootstrap color of the tag
    Possible values: , default, success, warning, important, info, inverse.
* `fields` - _optional_ - Fields to return separate by comas: name,id
* `limit` - _optional_ - Number of object to return (max 100, default 25)
* `limitstart` - _optional_ - Start of the return (default 0)
* `order` - _optional_ - ORDER by this field

### Add tags for a specific website

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website

### Update Joomla core on the remote site

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website

### Return uptime data

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website

### validate the site, return the new logs

> validate the site

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website

### validate the site, return the debug information

*Tags:* `sites`

#### Input Parameters
* `id` - _required_ - ID of the website

### Get a list of SSO Users

> Returns a list of SSO Users

*Tags:* `ssousers`

### Create a SSO User

*Tags:* `ssousers`

### Delete a specific SSO User

*Tags:* `ssousers`

#### Input Parameters
* `id` - _required_ - ID of SSO User that needs to be deleted

### Find SSO User by ID

> Returns a SSO User based on ID

*Tags:* `ssousers`

#### Input Parameters
* `id` - _required_ - ID of SSO User that needs to be fetched
* `fields` - _optional_ - Fields to return separate by comas: name,id

### Update a SSO User

*Tags:* `ssousers`

#### Input Parameters
* `id` - _required_ - ID of SSO User that needs to be updated

### Get a list of tags

> Returns a list of tags

*Tags:* `tags`

#### Input Parameters
* `name` - _optional_ - Do a 'LIKE' search, you can also use '%'
* `type` - _optional_ - Bootstrap color of the tag
    Possible values: , default, success, warning, important, info, inverse.
* `fields` - _optional_ - Fields to return separate by comas: name,id
* `limit` - _optional_ - Number of object to return (max 100, default 25)
* `limitstart` - _optional_ - Start of the return (default 0)
* `order` - _optional_ - ORDER by this field separete by comas. Add + / - after field for set ASC / DESC: type+,name-

### Create a tag

*Tags:* `tags`

### Get the list of fields

> Returns a list of fields

*Tags:* `tags`

### Delete a specific tag

*Tags:* `tags`

#### Input Parameters
* `id` - _required_ - ID of tag that needs to be deleted

### Find tag by ID

> Returns a tag based on ID

*Tags:* `tags`

#### Input Parameters
* `id` - _required_ - ID of tag that needs to be fetched
* `fields` - _optional_ - Fields to return separate by comas: name,id

### Update a tag

*Tags:* `tags`

#### Input Parameters
* `id` - _required_ - ID of tag

### Find sites by tag ID

> Returns a list of sites based with a specific tag id

*Tags:* `tags`

#### Input Parameters
* `id` - _required_ - ID of tag that needs to be fetched
* `name` - _optional_ - Do a 'LIKE' search, you can also use '%'
* `access_url` - _optional_ - Do a 'LIKE' search, you can also use '%'
* `j_version` - _optional_ - Do a 'LIKE' search, you can also use '%'
* `ip` - _optional_ - Do a 'LIKE' search, you can also use '%'
* `jUpdate` - _optional_ - Joomla core update
    Possible values: 1, 0.
* `published` - _optional_ - is published
    Possible values: 1, 0.
* `error` - _optional_ - have errors
* `nbUpdates` - _optional_
* `up` - _optional_ - is the website online
    Possible values: 1, 0.
* `fields` - _optional_ - Fields to return separate by comas: name,id
* `limit` - _optional_ - Number of object to return (max 100, default 25)
* `limitstart` - _optional_ - Start of the return (default 0)
* `order` - _optional_ - ORDER by this field separete by comas. Add + / - after field for set ASC / DESC: type+,name-

## License

**flow**ground :- Telekom iPaaS / watchful-li-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
