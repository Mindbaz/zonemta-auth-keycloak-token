# zonemta-auth-keycloak-token

Authentication with Keycloak for [ZoneMTA](https://github.com/zone-eu/zone-mta). Install this to performs SMTP authentication with [Keycloak](https://www.keycloak.org/) token

## Setup

Add this as a dependency for your ZoneMTA app

```
npm install @mindbaz/zonemta-auth-keycloak-token --save
```

Add a configuration entry in the "plugins" section of your ZoneMTA app

Example [here](./config.example.toml).

First enable plugin :

```toml
# auth-keycloak-token.toml
["modules/@mindbaz/zonemta-auth-keycloak-token"]
enabled="receiver"
interfaces=["feeder"]
```

Then set keycloak configuration for this plugin :

```toml
keycloak_url="http://example.org:8080"
```

## License

The GNU General Public License 3 ([details](https://www.gnu.org/licenses/quick-guide-gplv3.en.html))
