# photils-dt

A darktable plugin which tries to predict keywords based on the selected image. This plugin uses photils-cli to handle this task. Photils-cli is an application which passes the image through a neural network and generates a feature vector. This feature vector will be used to find similar images in a self-hosted online database and the corresponding tags. The usage of the feature vector has this advantage that at no time your selected image will leave the PC. Rather a representation of the image is sent.

![](docs/photils-dt.gif)

| Platform | Support            |
| -------- | ------------------ |
| Linux    | <center>✔️</center> |
| MacOS    | <center>✔️</center> |
| Windows  | <center>✔️</center> |

## Requirements
* photils-cli - https://github.com/scheckmedia/photils-cli

## Installation
* check the lua installation instructions - [https://github.com/darktable-org/lua-scripts](https://github.com/darktable-org/lua-scripts)
* copy photils.lua to contrib of lua-scripts
* copy photils.po to lua-scripts/locale/de_DE/LC_MESSAGES

## Usage
* Select an image
* Press "Get Tags"
* Select the tags you want from a list of suggestions
* Press "Attach .. Tags" to add the selected tags to your image