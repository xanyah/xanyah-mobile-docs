# Installation

## Requirements

* Yarn

## Installation

Clone the repo:

```text
$ git clone git@github.com:xanyah/xanyah-mobile.git
```

Once you've cloned the repo, enter the directory:

```text
$ cd xanyah-mobile
```

Install dependencies:

```text
$ yarn
```

To start the application, you can use the following commands with a device or simulator connected:

```text
$ yarn ios:dev             # To run on iOS
```

```text
$ yarn android:dev         # To run on Android
```

If somehow you're having trouble starting it, you can try the troubleshooting process available here:

{% embed data="{\"url\":\"https://facebook.github.io/react-native/docs/troubleshooting.html\#content\",\"type\":\"link\",\"title\":\"Troubleshooting · React Native\",\"description\":\"These are some common issues you may run into while setting up React Native. If you encounter something that is not listed here, try \[searching for the issue in GitHub\]\(https://github.com/facebook/react-native/issues/\).\",\"icon\":{\"type\":\"icon\",\"url\":\"https://facebook.github.io/react-native/img/favicon.png\",\"aspectRatio\":0}}" %}

## Additional steps for Android

You will need to create an environment file:

```text
$ cp .env.example .env
```

Generate a keystore file:

```text
$ keytool -genkey -v -keystore <path to keystore>.keystore -alias <keystore alias> -keyalg RSA -keysize 2048 -validity 10000
```

Then, update your `.env` with your keystore informations. You're now good to go!

