# covid19-supportnavi

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

## Overview

"covid19-supportnavi" is an open-source project that allows you to easily create a support information navigator by loading detailed administrative service information.
The covid19-supportnavi has the following features:

* Can use the same "search for the system that suits you" and "view the system by theme" functions as the "Support Information Navigator for COVID-19" of the Tokyo Metropolitan Government

* The administrative service information file can be prepared to easily update the data

* The navigation logic file can be prepared to easily update the logic

The differences from the "Support Information Navigator for COVID-19" of the Tokyo Metropolitan Government are as follows:

* Does not have the "search by keyword" function
* Does not have the "view the related information of the city/ward" function
* Does not have the "for medical personnel" menu

Please refer to the manual.pdf in the repository for more details on how to use it.

## Installation

First, copy all the files in the repository to your local machine.

If using a Git client, you can copy them with the following command:

```
git clone https://github.com/code4fukui/covid19-supportnavi.git
```

Next, install the dependent modules.

```
npm install
```

You can generate the entire set of site files with the following command.
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

## Update History

| Date | Version | Notes |
| ---- | ------- | ----- |
| 2021-11-12 | Initial | - |

## License

The covid19-supportnavi is provided under the MIT License. For details on the license, please refer to the license document ([LICENSE.md](LICENSE.md)).