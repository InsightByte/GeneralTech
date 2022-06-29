
## How to install MongoDB on Mac 

#### Install the Xcode command-line tools by running the following command in your macOS Terminal:

```xcode-select --install```


#### Download the official Homebrew formula for MongoDB and the Database Tools, by running the following command in your macOS Terminal:

```brew tap mongodb/brew```

#### Update Homebrew and all existing formulae:

```brew update```

#### Install MongoDB, run the following command in your macOS Terminal application:

```brew install mongodb-community@4.2```


#### Start MongoDB
```brew services start mongodb-community@4.2```

#### Stop MongoDB
```brew services stop mongodb-community@4.2```

#### Chech the MongoDB Service status 
```brew services list```

#### How to connect to a MongoDB 
This will use the default mongodb port

```mongo```

To use the mongo shell with custom port 

```mongo --port <your port name>```



