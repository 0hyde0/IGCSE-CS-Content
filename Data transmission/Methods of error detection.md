# Chapter 2.2: Methods of error detection

Objectives

```
Understand the need for error checking after data transmission and how they occur
Be able to describe processes involved in error detection methods
Be able to describe how a check digit is used to detect errors and identify examples of it in use, including ISBN and bar codes
Be able to describe how an ARQ can be used to establish that data is received without errors
```

## Damaged parcels

When you make a purchase online, there's a chance that the item you receive may be damaged due to mishandling during shipping, leading to frustration.

Similarly, when ``data is transmitted`` from one device to another, it ``can be affected by interference``, resulting in errors such as ``data corruption, loss, or gain.`` To address these issues, various error-checking methods are employed to determine if the transmitted data has been altered.

One such method is the ``parity check``, where an additional bit, known as the ``parity bit``, is appended to each unit of data. This method is relatively straightforward, as it involves ensuring that the total number of 1s in the data, including the ``parity bit``, is either even or odd. Both the ``sender and receiver need to agree on the type of parity`` being used. If the total number of 1s doesn't match the agreed-upon parity, an error is detected. However, this method has a limitation in that it cannot detect certain types of errors that maintain the same parity.

To combat this, a ``parity block check`` can be implemented, which, when combined with a ``parity byte check`` allows for error checking and the ability to pinpoint where. A parity block consist of a block of data with the amount of 1s totalled horizontally and vertically, where a parity byte is where the vertical parity bits are stored. 

Another alternative would be a ``checksum``, which is ``a value that is calculated using an algorithm`` on data, which can be a good indicator of whether the ``original data differs from the received data`` by ``recalculating the received data's checksum and comparing it to the original checksum``. ``Before transmission, a checksum of a data can be calculated and added to the data transmission`` and begins. When the checksum do not match, it can be assumed that an error has occured.

The last alternative would be an ``echo check``. This involves ``transmitting the received data back to the sender``, where ``it would then check for any errors within the data itself``. This ``isn't as reliable`` as ``an error could have occured during transmission to the sender or the receiver``. If an error does occur, the ``sender then transmits the data again.``

## Check digits

A ``check digit``, is another method of ``error checking`` for data. But it is more commonly used in bar codes, the ones that help supermarkets know what product is what with a single universal indicator. They are also used in ISBN (international standard book numbers).

A check digit is ``added to the end of a numerical sequence`` to ensure if the data is correct, which is calculated using ``standardised algorithms`` to ensure ``compatiblity``. 

An example of an ISBN code is here:

978-1-398-31828-**1**

The highlighted number is the check digit, from where when calculated based on the first 12 digits, indeed results in 1, which states that this ISBN code is valid.

Barcodes also work this way, the number sequence is read by a barcode scanners based on the distance of the lines of the barcode by shining a laser on the black and white lines which reflects light back to the scanner. And usually, the final digit on a barcode is the check digit, which can again be used to authenticate an item.