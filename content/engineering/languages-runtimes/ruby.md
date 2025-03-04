---
title: Ruby guide
sidenav: true
sticky_sidenav: true
permalink: /engineering/languages-runtimes/ruby/
redirect_from:
  - engineering/ruby/
tags: engineering
layout: layouts/page
eleventyNavigation:
  parent: engineering_languages
  key: Ruby
  order: 5
  title: Ruby
subnav:
  - text: Style guide
    href: "#style-guide"
  - text: Testing
    href: "#testing"
---
Help us make this section better by [submitting an issue](https://github.com/18F/guides/issues/new) or joining us in the [#ruby](https://18f.slack.com/messages/ruby/) channel!

A guide for writing and maintaining Ruby and Rails applications

## Style guide
Follow the [Ruby style guide](https://github.com/bbatsov/ruby-style-guide) and enforce it via static analysis tools such as [Code Climate] and [Rubocop]. You can copy the [recommended Rubocop configuration]({{ "/assets/engineering/dist/rubocop.yml" | url }}) in your Ruby project and make any changes based on your team's preferences.

Note that the Rubocop configuration linked above only includes settings that differ from the default configuration. We tend to agree with most of the default settings.

Whenever a `Style` Rubocop setting provides multiple options, at least one option must be chosen. A cop that supports different styles must never be disabled outright. The point is to pick one style and use it consistently.

## Testing

### Validating HTML output
We use HTMLProofer for testing rendered HTML automatically. Please see the [test page] for more details.

[Code Climate]: https://codeclimate.com
[Rubocop]: https://github.com/bbatsov/rubocop
[test page]: /engineering/tools/tests/
