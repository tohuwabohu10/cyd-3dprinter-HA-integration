# Changelog

All notable changes to this project will be documented in this file.

## Unreleased

- Convert print start/end times from UTC timestamps to the Home Assistant local timezone so they match the header clock.
- Treat ISO-format Bambu timestamps without an explicit offset as UTC, and derive end time from remaining duration when a print is active so it matches the ETA.
- Capture print start time on the CYD when print status first switches to Preparing or Running, instead of using the unreliable Bambu `start_time` sensor.
