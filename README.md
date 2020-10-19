# env_loader
The package looks up necessary environment variables and use them to set settings for application.

The settings must be formed as struct with byte and string fields.

Warning: This package is considered as deprecated and will not be updated in the future.

Example:

```go
...
type EnvironmentSettings struct {
	Port       string `env:"PORT validate:"numeric"`
	Database   string `env:"DATABASE"`
	CacheSize  byte `env:"CACHE_SIZE"`
	LaunchMode string `env:"LAUNCH_MODE"`
}
...
```
