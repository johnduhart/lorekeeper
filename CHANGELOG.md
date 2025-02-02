# 2.1.0
* Modify SimpleLogger to properly log exceptions with named parameters

# 2.0.0
* Set `mode: :compat` in Oj.dump to stringify keys
* Support Ruby 3.1
* Drop support for Ruby < 2.5.0

# 1.12.0
* Remove ZipkinTracer information from stacktrace output
* Move CI to GitHub Actions

# 1.11.1
* Modify FastLogger#add to log progname as a message if no message and block are given

# 1.11.0
* Support for activerecord-session_store v2 which calls only silence and not silence_logger

# 1.10.0
* Use ActiveSupport::BacktraceCleaner to reduce noise in stacktrace output

# 1.9.0
* Remove Newrelic instrumentation information from stacktrace output

# 1.8.0
* Allow to use named parameters in the .exception method

# 1.7.2
* Add a second parameter to respond_to? to avoid Ruby 2.6 warnings
* Drop support for unsupported Ruby 2.1 and Ruby 2.2

# 1.7.1
* Ensure `data` is not nil when logging wrong #exception usage

# 1.7.0
* Add the `level` property to the JSON Logger output

# 1.6.2
* Update oj gem to resolve segmentation fault issue

# 1.6.1
* Update reference to OJ gem to support Ruby 2.4

# 1.6.0
* Adds 'exception' to simple logger to unify APIs

# 1.5.1
* Updating version to resolve issue with mistakenly created 1.5.0 gem version

# 1.5.0
* Mistakenly created version, please disregard

# 1.4.1
* Change array creation syntax to support Ruby 1.9

# 1.4.0
* Adds '_with_data' to the simple logger so we can display data in the terminal
* Adds 'respond_to?' to the multilogger so users can check capabilities of the loggers

# 1.3.1
* Loggers provide an inspect method to avoid being too noisy on outputs

# 1.3.0
* Time in the JSON output specifies microseconds.
* Using 'Z' to specify the UTC timezone instead of +0000 as per ISO 8601.
* Debug and Info messages use the default foreground color of the terminal.

# 1.2.1
* If a file does not exist, it will create it on behalf of the application

# 1.2
* Added a silence_logger method to the logger. For compatibility with activerecord-session and maybe other gems.

# 1.1.1
* Avoid syntax errors in rubies < 2.3

# 1.1.0
* Added an 'add' method to the logger so it is compatible with the Logger provided by Ruby's standard library

# 1.0.0
* Initial release
