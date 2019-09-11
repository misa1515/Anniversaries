# Anniversaries
The 'anniversaries' component is a Home Assistant custom sensor which counts down to a recurring date such as birthdays, but can be used for any anniversary which occurs annually on the same date.

The state is the number of days remaining to the next occurance.

The years attribute shows how many years have passed since the first occurance (ie, age)

## Configuration
Add `anniversaries` sensor in your `configuration.yaml`. The following example adds two sensors - Shakespeare's birthday and wedding anniversary!
```yaml
# Example configuration.yaml entry
sensor:
  - platform: anniversaries
    name: Shakespeare's Birthday
    date: '1564-04-23'
  - platform: anniversaries