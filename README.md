# Installation

 * Install `ruby-2.5`
 * Install `bundler`
 * `bundle install`


# Running

The CLI app requires the `CLIENT_ID` and `CLIENT_SECRET` environment variables to be set. You can either set them in your environment and call the app using:

```sh
> bundle exec scientist
```

Or you can specify them at run time:

```sh
> CLIENT_ID=ABC CLIENT_SECRET=XYZ bundle exec scientist
```

Running without parameters will print help documentation:

```
Commands:
  scientist categories                  # Load the categories
  scientist category_wares BEACON_SLUG  # Load wares by category
  scientist help [COMMAND]              # Describe available commands or one specific command
  scientist provider PROVIDER_ID        # Load a provider given an id
  scientist provider_wares PROVIDER_ID  # Load a provider's wares given an id
  scientist providers <SEARCH STRING>   # Find providers (search string optional)
  scientist stress                      # Stress test the system
  scientist token                       # Get client credentials token
  scientist ware WARE_ID                # Load a ware given an id
  scientist ware_providers WARE_ID      # Load a ware given an id
  scientist wares <SEARCH STRING>       # Find wares (search string optional)

Options:
  [--quiet], [--no-quiet]
  [--raw], [--no-raw]
```
