# Chapter 1.2: Text, sound, images

Objectives

```
Understand how and why computers use character sets
Understand how and why a computer represents sounds and images
```

## ASCII and Unicode

The ``character set`` any programmer in the US from the 1980s until today would've known is ASCII. Most notably because it was the default ``set of characters`` a lot of the computers there used.

A list of characters found in ASCII can be found below.

| Index | Character |
|-------|-----------|
| 0x30  | 0         |
| ....  | 1-8       |
| 0x39  | 9         |
| 0x41  | A         |
| ....  | B-Y       |
| 0x5A  | Z         |
| 0x61  | a         |
| ....  | b-y       |
| 0x7A  | z         |

However, ASCII wasn't adapted to allow computers to display letters or characters from other languages. Because of this, ``Unicode`` is formed and maintained by the Unicode Consortium to support all writing systems.

In a nutshell, Unicode adds support for symbols and a greater range of characters than ASCII. This comes at the cost of requiring more bits per character than ASCII.

Note:
```
Text is converted into binary to be processed by a computer.
```

## Wiggly waves

Computers, as always, would need every data converted into binary. This also applies to sound.

``Analog`` sound waves are ``sampled``, which means measuring the ``amplitude`` of them. Each ``sample`` generates a value and can be represented in binary for a computer to process.

``Sample rate`` is the number of samples taken per second, measured in Hz (hertz). 1Hz is equal to 1 sample of the sound wave.

``Sample resolution`` is the number of bits per sample.

The audio file size and accuracy increase and decrease according to how high the sample rate and resolution are.

## Blocky colours in a grid

Ever wonder why images can sometimes look a bit choppy?

This is because of how "images" are made. Images consist of a series of pixels in a grid. When the ``resolution`` of an image changes in size, so will the quality and size of the image.

The colours in an image are also important. Color depth controls how accurate the color of each pixel is, in bits. Again, this also affects the quality and size of the image.

In a nutshell, the quality and size of the image increase and decrease according to the colour depth and resolution.