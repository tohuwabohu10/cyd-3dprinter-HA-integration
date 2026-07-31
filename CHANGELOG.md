# Changelog

All notable changes to this project will be documented in this file.

## Unreleased

- Convert print start/end times from UTC timestamps to the Home Assistant local timezone so they match the header clock.
- Derive end time from `now + remaining` during active prints so it matches the ETA, using the same unit conversion as the ETA label.
- Capture print start time on the CYD when print status first switches to Preparing or Running, instead of using the unreliable Bambu `start_time` sensor.
