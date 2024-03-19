# [← Back to repo list](https://github.com/64bit-polygon/links)

# Applanga service

## Background

In 2021 the company I worked at switched their localizations / translations platform from an old clunky platform to <a href="https://www.applanga.com/">`Applanga`</a>. This was a big shift since as a global company, all of our user-facing text is delivered via a translations platform.

This new start provided an opportunity to provide a standard way of incorporating the translations data across many teams and platforms. In service of this I created two projects that can work and tandem or separately depending on the needs of the teams.

## Description

Getting our localization content quickly is key. As such, we do not want all of our users to constantly be triggering calls to `Applanga` directly. To optimize delivery, it makes sense to store all the translations on a node server server and hit that instead. `Applanga service` does that: it caches and refreshes our translations on a server we control. Additionally, the raw data we get from `Applanga` is not structured optimally for our needs. The response object is needlessly complex out of the box. So along with caching the data, it also transforms it into a much simpler structure.