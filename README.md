# als-oracle-pathfinder
An Account Lookup Service Oracle for GSMA Pathfinder resolution of MSISDNs. Code based on the
Mojaloop [ALS Oracle Template](https://github.com/mojaloop/als-oracle-template).

## TODO
* NOTE THAT MANY OF THESE TODOS PROBABLY APPLY TO THE MERCHANT ORACLE ALSO
* HANDLE CURRENCY IN RETURN VALUE CORRECTLY!
* add merchant id regex validation to merchant oracle swagger
* import openapi validation? port swagger to openapi?
* import header validation
* handle currency querystring in get participants by type and id?
* remove secrets from config, then squash down to initial commit. Replace config mechanism with
    dotenv, .template.env and .env entry in gitignore to prevent secrets being committed
* pre-commit hook to run tests before commit (https://www.npmjs.com/package/pre-commit or DIY)
* tidy up pathfinder lib config- it should allow a user to supply a pathfinder config and provide
    any missing defaults
* pathfinder module should use this.logger.{error, warn, info, debug}
* go through and address all TODOs in pathfinder lib
* use dotenv? inside config.js?
* make sure pathfinder tests are running
* bring in validation libs; hapi-openapi is considerably lacking
* if there is an error in server init, the server hangs forever. Try to throw an error from, for
    example, the db init method. This could be pretty annoying for deployment.
