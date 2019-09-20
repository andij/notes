---
description: Here I can test the release notes!
---

# Release notes

## Version [X.X.X]

**[briefly descibe the release]**

Release date - [YYYY-MM-DD]

**What’s new around here [add emoji]**

**[add an emboldened line if there's more than one list]**

* [include a list of things]
  * [second level item]
  * [wrap `ns-component` names and `code` references in backticks]
* [title followed by - http://the.url-of.choice]

**[add an emboldened line if there's more than one list]**

* [include a list of things]
  * [second level item]
  * [wrap `ns-component` names and code references in backticks]
* [title followed by - http://the.url-of.choice]

**Bug fixes [add emoji]**

* [include a list of things]
  * [second level item]
  * [wrap `ns-component` names and code references in backticks]
* [title followed by - http://the.url-of.choice]

**Improvements [add emoji]**

* [include a list of things]
  * [second level item]
  * [wrap `ns-component` names and code references in backticks]
* [title followed by - http://the.url-of.choice]

**Feedback [add emoji]**

All our Requests For Change can be found in our Requests project board in Github.
https://github.com/ConnectedHomes/nucleus/projects/6

Any questions? Let us know 🙌🏼


## Version 1.1.4

**Additional components, bugfixes and improvements**

Release date - 2019-07-31

**What’s new around here 🕑**

* A Landmark variant `hillside` which is less promotional than `summit`
  * It has no image and no call to action.
* `ns-form` - The container for all `ns-inputter` components which manages the validation.
* Introducing the `select` variant of `ns-inputter` commonly known as - the dropdown.

**Bugfixes 🦋**

* Addressing an issue where the BG-VI.css anchor styles were overriding Nucleus.
* Ensuring that `ns-cta` is tabbable when not contained within an `<a>`.
* Slight change to the implementation of the CSS box model.
* Adding slot styling to the heading within the `flat` variant of `ns-card`.

**Improvements 🐶**

* Validation improvements to `ns-inputter` suppoting minLength, maxLength and isBetweenLength validations.
* Validation for radio buttons and `ns-inputter` `select` component.
* Deprecated "Key" variant from the `ns-cta` component.
* The default Landmark has been renamed from `hub` to `summit`.
* The `ns-cta` within `ns-lockup` and `ns-landmark` is now optional.
  * Choose 'none' from the 'CTA type' dropdown in the Knobs addon.

**Feedback 🦉**

All our Requests For Change can be found in our Requests project board in Github.
https://github.com/ConnectedHomes/nucleus/projects/6

Any questions? Let us know 🙌🏼


## Version 1.1.3

**Bugfixes and improvements**

Release date - 2019-06-24

**Sketch Library 🐳**

* Fixed broken and duplicated Components / Templates.

**Bugfixes 🏏**

* Fixed the inconsistent positioning of the accordion chevron when multiple expanders were used.
* Addressed the IE11 bug where the incorrect text colour appeared within `ns-cta` and `ns-tab`.
* Enable the position `right` for the circle decoration.
* Fix initial value overwrite in `ns-inputter`.

**Improvements 🌻**

* Removed `slot="label"` from `ns-inputter` as we use the anonymous slot.
* Improve the `ns-tabs` Storybook story.
* Include the tap illustration.
* Adding the solid and outline Energy icon.

**Feedback 🦕**

All our Requests For Change can be found in our Requests project board in Github.
https://github.com/ConnectedHomes/nucleus/projects/6

Any questions? Let us know 🙌🏼


## Version 1.1.1

**Something for you, you and you! 🎉**

Release date - 2019-06-11

**What’s new around here 🌶**

* `ns-inputter` - the vanilla first of our form elements.
  * Text, Email, Telephone, Password, Number, Radio, Checkbox.
  * Field-level validation.
  * Placeholder.
  * Helper text.
  * Helper details.
* `ns-video` - include a YouTube video into a lockup.
* `ns-tab` - the tab that lives within tabs.
* `ns-tabs` - include a few tab to make a tabs.

**Sketch Library**

* Release 2.0 - (Out of Pre-release).
  * Download the latest: https://github.com/ConnectedHomes/centrica-ux/releases.
* Added Guides to give indication of where components can be placed.
* Included Templates to quickly mockup a page and placing components in a layout.

**Bugfixes 🐞**

* Replace previous green outline on `ns-cta` with current yellow outline.
* Ensuring that the class of `blur` is implemented when required.
* Address the removal of `margin-bottom` on the last element.
* Improve specificity of typographic styling.
* Including robust techniques for setting attributes.

**Improvements 🌸**

* Storybook, split Playground and Foundations.
* Remove unused properties from our components.
* Setting a white background to `ns-expander` within `ns-accordion`.
* Including a variable for `@outline` colour.
* Adding the solid and outline Rewards icon.

**Collaboration 🤗**

A big thank you to everyone involved in contributing to this release!

* OAM - for their collaboration throughout this release.
* Energy Sales - for working with us to run a joint user testing session using a Nucleus coded prototype.
* New Boilers - For collaborating with us to make sure their recent journey contained Nucleus components.
* Help & Support - for their patience with the Nucleus CMS page, allowing us time to build the video component.

**Feedback 🐢**

All our Requests For Change can be found in our Requests project board in Github.
https://github.com/ConnectedHomes/nucleus/projects/6

Any questions? Let us know 🙌🏼


## Version 1.0.0

**Our first major release! 🎉**

Release date - 2019-04-15

**What’s new around here 🌶**

**Integration with Ember Commons**
* A feature flag exists in Ember Commons to enable Nucleus.

**Sketch Nucleus Pattern Library**
* Added all available icons.
* Added Accordions.
* Added more screen sizes to each Component.

**Documentation**
* Becoming Nucleus - https://docs.britishgas.design/community/becoming-nucleus
* Best practices - https://docs.britishgas.design/community/best-practices
* Events - https://docs.britishgas.design/community/events
* Modular scale - https://docs.britishgas.design/foundation/modular-scale
* Typography sizes - https://docs.britishgas.design/foundation/typography
* Optimise your images - https://docs.britishgas.design/foundation/photography
* Our documentation - https://docs.britishgas.design
* Accordion - https://docs.britishgas.design/components/ns-accordion

**Bugfixes 🐞**

* Vertical spacing adjustments.
* Adjusting the style of the heading within our Accordion.
* Setting all Actions to be 100% width at small screen.
* Removing the duplicate BG Flame font loading.
* Fixed the hierarchy of the screen sizes in Sketch library.

**Feedback 🐳**

The following request for changes have been started

* Main navigation - https://github.com/ConnectedHomes/nucleus/issues/491
* Tab panel - https://github.com/ConnectedHomes/nucleus/issues/587
* Selection cards - https://github.com/ConnectedHomes/nucleus/issues/582
* Form fields - https://github.com/ConnectedHomes/nucleus/issues/579

All our Requests For Change can be found in our Requests project board in Github.
https://github.com/ConnectedHomes/nucleus/projects/6

Any questions? Let us know 🙌🏼
