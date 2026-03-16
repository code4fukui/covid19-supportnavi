# covid19-supportnavi

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

"covid19-supportnavi" is an open-source project that allows you to easily create a support information navigator by loading detailed administrative service information.

## Features

- Can use the same "search for the system that suits you" and "view the system by theme" functions as the "Support Information Navigator for COVID-19" of the Tokyo Metropolitan Government
- The administrative service information file can be prepared to easily update the data
- The navigation logic file can be prepared to easily update the logic

## Installation

First, copy all the files in the repository to your local machine. If using a Git client, you can copy them with the following command:

```
git clone https://github.com/code4fukui/covid19-supportnavi.git
```

Next, install the dependent modules:

```
npm install
```

You can generate the entire set of site files with the following command:

```
npm run build
```

The files will be generated in the `dist` folder.

## Usage and Customization

### Setting the list of service information

Refer to "About the administrative service information csv" in the manual.pdf.

### Setting the navigation data

Refer to "About the navigation logic csv" in the manual.pdf.

### Changing the color scheme

You can change the color scheme by editing the following CSS files:

- static\styles\color-def-dark.css
- static\styles\color-def-default.css
- static\styles\color-def-light.css

## License

MIT License — see [LICENSE](LICENSE).