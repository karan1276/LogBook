![alt tag](docs/logo.png)

# angular2-log-book

## Installation

To install this library, run:

```bash
$ npm install angular2-log-book --save
```
## Usage

### Installation

To install this library, run:

```bash
$ npm install angular2-log-book --save
```

### Adding library

Add the library in your angular 2 project. If you are following the [Angular 2's Quickstart Guide]    (https://angular.io/docs/ts/latest/quickstart.html) it should be something like this:
```bash
        import { NgModule }      from '@angular/core';
        import { BrowserModule } from '@angular/platform-browser';
        import { AppComponent }  from './app.component';
        import { Log } from "angular2-log-book/core"; // <-- ADD THIS
    
        @NgModule({
            imports:      [ BrowserModule ],
            declarations: [ AppComponent ],
            bootstrap:    [ AppComponent ],
            providers:    [ Log ] // <-- AND THIS
        })
        export class AppModule { }
```
## Development

To generate all `*.js`, `*.js.map` and `*.d.ts` files:

```bash
$ npm run tsc
```

To lint all `*.ts` files:

```bash
$ npm run lint
```

## License

MIT © [Karan Sharma](karan1276@gmail.com)
