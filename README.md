# kintone-field-migration-tool-plugin
Migrate data from one field type to another type.

# Notes
 Create Kintone plugin:
Data Migration Tool: in the plugin settings page:

Given a source field (with data) and a target field (empty in all records) of the same type in the same app [or a different app?], copy all the data from the source field into the target field. Provide an option to delete the source field.

Given a source field (with data) and a target field (empty in all records) of a different type, copy all the data from the source field into the target field. Provide an option to delete the source field.

Single-line text -> Multi-line text
Single-line text -> Rich text
Single-line text (all strings in all records must resolve to number, and indicate what the problem records are… can we fix it on this plugin settings page? would be awesome!) -> Number
Single-line text -> Drop-down
Single-line text -> Radio button
Single-line text -> Multichoice
Single-line text -> Check box
Single-line text -> Lookup (???)

Lookup -> Lookup (???) (indicate the problem record and allow resolution on the plugin settings page if possible)

Multi-line text -> single-line text
Multi-line text -> rich text

Number -> Single-line text

Drop-down -> Radio button
Drop-down -> Check box
Drop-down -> Multichoice

Radio button -> Drop-down
Radio button -> Check box
Radio button -> Multichoice

Check box -> Multichoice
Check box -> Radio button (indicate problem records where multiple items are checked… let’s be able to fix it on this plugin settings page… allow all fixes to be done at once and saved instead of one at a time, since there may be an issue in the later records that would have a person reconsider migrating to this field)
Check box -> Drop-down (indicate problem records where multiple items are checked… let’s be able to fix it on this plugin settings page… allow all fixes to be done at once and saved instead of one at a time, since there may be an issue in the later records that would have a person reconsider migrating to this field)

Multichoice -> Check box
Multichoice -> Radio button (indicate problem records where multiple items are checked… let’s be able to fix it on this plugin settings page… allow all fixes to be done at once and saved instead of one at a time, since there may be an issue in the later records that would have a person reconsider migrating to this field)
Multichoice -> Drop-down (indicate problem records where multiple items are checked… let’s be able to fix it on this plugin settings page… allow all fixes to be done at once and saved instead of one at a time, since there may be an issue in the later records that would have a person reconsider migrating to this field)


Date -> Date and time (indicate that time will be resolved in bulk as 12:00:00 UTC (midday))

Date and time -> Date (drop the time and warn it will be dropped)