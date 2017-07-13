# docker-registry-cli

This is very-basic python built script that interacts with private docker registries that are setup us to use basic auth. The tool can list all repos, images, tag & optionall all FS layers that make an image. A image can be deleted& an exclude list can be provided to exlude certain images from deletion.

## Getting Started

Simply get this script & run.

### Prerequisites

You need to know URL of your registry & the username & password used

### Installing

No special steps needed to install anything - as long as you have python - you are all set

### Running

```
docker-registry-cli -h

Usage: ./docker-registry-cli [-s server] [-u username] [-p password] [-v verbose] [-d delete] [-e EXCLUDE]
  -s   --server            Docker registry URL
  -u   --username          docker registry user-name
  -p   --password          docker registry user's password
  -v   --verbose           verbose output
  -d   --delete            deletes ALL images, provide exclusions via -e flag
  -e   --exclude           list of repos to exclude comma-separated list, name:tag format

example: ./docker-registry-cli -s 139.156.121.159:5000 -u admin -p p@ssword -v true -d true -e foo:bar,foo1:bar1

```

## Built With

* [Python](http) - Python

## Contributing

Feel free to extend the script share as you desire.

## Versioning

I highly encourage use of [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Sachin Dhamdhere** - *Initial work* - [Sachin Dhamdhere](https://www.linkedin.com/in/sachindhamdhere/)

## License

This project is licensed under the MIT License - the text of which roughly goes as ...

```
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```


## Acknowledgments

* [Drupad Panchal](https://www.linkedin.com/in/sachindhamdhere/)  inspired parts of this script 

