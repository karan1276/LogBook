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
        import { LogBook } from "angular2-log-book/core"; // <-- ADD THIS
    
        @NgModule({
            imports:      [ BrowserModule ],
            declarations: [ AppComponent ],
            bootstrap:    [ AppComponent ],
            providers:    [ LogBook ] // <-- AND THIS
        })
        export class AppModule { }
```

### Use it
        @Component({
            ...
        })
        export class AppComponent(){
            constructor( private $log: LogBook ){
                this.log.error('This is a priority level 1 error message...');
                this.log.warn('This is a priority level 2 warning message...');
                this.log.info('This is a priority level 3 warning message...');
                this.log.verbose('This is a priority level 4 debug message...');
                this.log.debug('This is a priority level 5 log message...');
                this.log.silly('This is a priority level 6 log message...');
            }
        }
## Features

### Supports log levels:
Supported log levels are `error`, `warn`, `info`, `verbose`, `debug` and `silly`. To log at a certain level write:
```bash
this.log.level_name('Hello world!');
```
replace `level_name` with `error`, `warn`, `info`, `verbose`, `debug` and `silly`.
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
