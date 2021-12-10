# wordpress-to-github implementation for cannabis.ca.gov

This is the [wordpress-to-github](https://www.npmjs.com/package/@cagov/wordpress-to-github) implementation for [cannabis.ca.gov](https://cannabis.ca.gov).

## Deploys services to the following Azure Function

- `FA-GO-WORDPRESS-TO-GITHUB-CANNABIS-CA-GOV` - Function app
- `sagowpghubcannabiscagov` - Storage account

## Target site source

https://github.com/cagov/cannabis.ca.gov

## Referenced WordPress instances

- https://live-cannabis-ca-gov.pantheonsite.io/wp-admin/

## WordPress notification config target

You will need to create a Function Key in the Azure instance to use a trigger. See the [wordpress-to-github readme](https://github.com/cagov/wordpress-to-github#readme).

### Trigger Target

`https://fa-go-wordpress-to-github-cannabis-ca-gov.azurewebsites.net/WordpressSyncHttpTrigger?code=[Put Function Key Here]`

## Current Configuration

See the [endpoints.json](https://github.com/cagov/services-wordpress-to-github-cannabis-ca-gov/blob/main/WordpressSync/endpoints.json) file in this project for current configuration.
