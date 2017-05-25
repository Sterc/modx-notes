# MODX Meetup Malta - The Ultimate CMS Interface
These notes are taken from the MODX Meetup Malta on May 13th, 2017. These findings are from a group varying from experienced MODX developers to people who saw MODX for the first time. This information is intended to create a better user experience for MODX.

The results below are categorised by group. Some overlap might exist.

## People don't know where they are
New users don't know where to go. They experience a lack of guidance within the manager experience. Improvements could be:

- More descriptions for input fields.
- Tooltips for important functionality for first-time users. Small guide using tooltips. Not too many, just a couple of to get people started.
	- Note: it shouldn't be necessary to have tooltips. It kind of means that the interface isn't intuitive enough.
- MODX currently is made from a developer-perspective. It is hard to make it more user-centric in its current form. Plans are made to change this in MODX Next, where there will be different UI for different groups.
- Resource-lists could use improvements: mention the breadcrumb in the dropdown-resource-list. **Needs mockup.**

## User testing is easy
There hasn't been much user-testing for MODX. We experienced how easy it is. Just ask random people who aren't used to working with MODX and give them some tasks in MODX.
- Golden rule: Don't ask team members!
- Explore the possibility of offering Hotjar-tracking when installing MODX.

## A lot of features/buttons exist in MODX, which long-time MODX users are unaware of
Did you know the resource edit page has a help button on the top-right?
- Lack of color-use for buttons.
- All MODX buttons should be reviewed
- Use more colours in the manager for buttons (green for save, red for cancel, grey for close)
- Use more icons for buttons (possibly combine text with icons - research needed on this)
- Bin icon is unclear. Looks like a delete button. Symlink looks like a duplicate button.
- We have 5 create buttons (resource, symlink, etc) on top of the resource-tree but the create-resource is used most of the times. We should replace that with one 'Create' button with a small downarrow with more options.
- Creating a new page should have this workflow: enter page title, select parent folder, select template (including preview). After this you get the resource-pane with more options. This prevents the evil reload-page-for-template-change.

## To much feature-overwhelm in the manager. Four ways to create a new resource. Too many options
- Stick to less options which actually work
- Show only what is used a lot. E.g.: resource-edit will only show save/view + more button with other options (remove/close/duplicate/help)
- The help-buttons should be removed. There shouldn't be two help-buttons at the same time.
- Help should be context-specific (so show help about what you're doing now).

## Template chooser with visual preview of the template before continuing editing
- When you create a resource and you change the template, it reloads the whole page. In most cases you don't really know what the template looks like (for example if you don't use the CMS every day).
- The new process would be: create a new resource, have a blank page with a template-picker which shows a list of all the available templates on the left. Clicking a template on the left, shows a preview of the template on the right (these previews would be images/screenshots uploaded manually by the developer). This saves time and frustration.
- There is a [concept for a future "template chooser"](https://github.com/jpdevries/modx-create-resource#modx-create-resource) which originated at the Malta meetup being actively developed.

## There is a real difference between creating and editing a page
- You probably only fill in the pagetitle/description/introtext/template when creating a page. But when you edit a page you want to go straight to the content-editor, but first you have to scroll past the meta-data.
- Rearrange the fields.
- Also rearrange the labels/input fields (near each-other instead of below each-other)
- Have the resource-tabs fixed (document/settings/tvs, but also save/view buttons)

## Too much information (like page ID's)
- There is a system setting to hide ID's
- Tooltips for input fields
- Maybe show ID on-hover

## Setup is too complicated and hard to understand
- Remove a lot of developer-info in the setup
- Enable the user to select a pre-build template (blog/portfolio/etc)
- Inform the user what is happening and prevent hitting install twice.
- Mention the MODX framework more. We don't only build websites with it. There should also be an App-distribution.
