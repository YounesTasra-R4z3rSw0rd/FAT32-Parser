# FAT32 Filesystem Parser
This python script is a FAT32 filesystem parser that allows you to analyze and parse FAT32 filesystems.

## Options
```
       -h, --help                               - Print out the help menu
       -i, --image  IMAGE                       - Enter the path to the file system raw image
       -m, --mbr                                - Parse Master Boot Record (MBR) only
       -p, --partition                          - Select the partition number (from 1 to 4) for which you would like to retrieve the boot sector information.
       -v, --verbose                            - Print out a quick documentation of every parsed field
```

## Usage
#### Parsing Master Boot Record only:
```bash
$ python3 --image /path/to/image --mbr 
```
![1](https://user-images.githubusercontent.com/101610095/232246774-44cbe18f-ceaa-4c57-a505-ddddcd545fd8.gif)

* Using verbose Mode:
```bash
$ python3 --image /path/to/image --mbr --verbose
```
![2](https://user-images.githubusercontent.com/101610095/232246865-af0ef9df-58c1-4ab2-b048-c351e0057ffa.gif)

#### Parsing the entire disk image:
```bash
$ python3 --image /path/to/image
```
![3](https://user-images.githubusercontent.com/101610095/232247263-66e09adc-5b7a-4150-861f-98617219fa2f.gif)

* Using verbose mode:
```bash
$ python3 --image /path/to/image --verbose
```

#### Parsing the boot sector of a specific partition
```bash
$ python3 --image /path/to/image -p [1-4]
```

## Requirements
```bash
$ pip3 install -r requirements.txt
```

## Contributing
Contributions are welcome! If you'd like to contribute to this project, please fork the repository and submit a pull request with your changes.

## License
This project is licensed under the MIT License - see the [License](https://github.com/YounesTasra-R4z3rSw0rd/FAT32-Parser/blob/main/LICENSE) file for details.
