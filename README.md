# can-npm-publish

A command line tool that check to see if `npm publish` is possible.

## Check list

- [ ] Check that the package is not `private:true`
- [ ] Check that `pacakge@version` is already published in npm registry

## Install

Install with [npm](https://www.npmjs.com/):

    npm install can-npm-publish

## Usage

Run `can-npm-publish` before `npm publish`:

    can-npm-publish && npm publish
    
### UseCase

You can use it for publishing without choice.
For example, it is useful for using with [lerna](https://github.com/lerna/lerna "lerna").

Publish all packages if it is possible.

    lerna exec -- can-npm-publish && npm publish

## Changelog

See [Releases page](https://github.com/azu/can-npm-publish/releases).

## Running tests

Install devDependencies and Run `npm test`:

    npm i -d && npm test

## Contributing

Pull requests and stars are always welcome.

For bugs and feature requests, [please create an issue](https://github.com/azu/can-npm-publish/issues).

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## Author

- [github/azu](https://github.com/azu)
- [twitter/azu_re](https://twitter.com/azu_re)

## License

MIT © azu