# Sample Swagger

This is a sample Swagger API Project

## Development

This project is a [Node](https://nodejs.org/en) project managed by the [Yarn](https://yarnpkg.com/) package manager.
It runs JavaScript and is bundled using [Webpack](https://webpack.js.org/)

### Install dependencies

You need to install the dependencies for the project.

```
% yarn intsall
```

### Building

To build the project run the following command

```
% yarn build
```

this will package the project into bundle.js

### Run

```
% yarn dev
```

The SwaggerUI should now be available on [http://localhost:8080/](http://localhost:8080/)


## Code Generation

Install [swagger-codegen](https://github.com/swagger-api/swagger-codegen).

### Generate Server Code

#### (If necessary) install Java Runtime
Make sure you have the Java Runtime (JDK) intalled on your machine

e.g.

```
%java -version
```

if you see the following message

```
The operation couldn’t be completed. Unable to locate a Java Runtime.
Please visit http://www.java.com for information on installing Java.
```

you need to install the Java Runtime on your machine.

A successful message will look something like this

```
% java -version
openjdk version "21.0.3" 2024-04-16
OpenJDK Runtime Environment Homebrew (build 21.0.3)
OpenJDK 64-Bit Server VM Homebrew (build 21.0.3, mixed mode, sharing)
```

#### (If necessary) source your `JAVA_HOME`

Make sure you have defined your `JAVA_HOME` and that it's in your `PATH`

for a *nix environment source teh `dev.sh` file

```
% source dev.sh
```

#### Run Codegen

Run the codegen command and specify the language

```
% yarn run codegen:[lang]
```

e.g. for Java

```
% yarn run codegen:java
```

and you can see that it generate the code in `./dist/java`