# Chapter 1.3: Data storage and compression

## Bytes to Exbibyte

Because computers have limited space, just like in the real world, we have a unit of measurement to see how large a storage medium would be.

The units and their size are given below.

| Unit       |  Short unit  |  Size in bytes       | Size in previous denomination |
|------------|--------------|----------------------|-------------------------------|
| Bytes      |  B           |  2^2                 | 8 bits                        |
| Kibibytes  |  KiB         |  2^10                | 1024 B                        |
| Mebibytes  |  MiB         |  2^20                | 1024 KiB                      |
| Gibibytes  |  GiB         |  2^30                | 1024 MiB                      |
| Tebibytes  |  TiB         |  2^40                | 1024 GiB                      |
| Pebibyte   |  PiB         |  2^50                | 1024 TiB                      |
| Exbibyte   |  EiB         |  2^60                | 1024 EiB                      |

In the actual exam, you **MUST** use 1024 as a standard measuring constant for calculating file (audio or image, with information such as ``colouring depth``, ``resolution``, ``sampling resolution``, and ``sampling rate``) sizes in the exam.

## Compression

When we compress an object, we allow ourselves to free up more physical space to store said object. However, when we try to restore the object to its original shape, sometimes it may look a little deformed. This can also be said for ``lossy`` compressed files.

Lossy compression is the best type of compression when it comes to reducing file size as much as possible, by permanently removing data. An example would be reducing resolution and color depth for images, and sample rate or resolution for audio.

If one had to compress an important document, however, lossy compression isn't going to be an option due to how it permanently removes data. This is where ``lossless`` compression comes in. It allows for the compression of data without a fraction of it being permanently lost. A method of lossless compression would be RLE (run length encoding).

The reason ``compression`` exists, again, is to reduce the size of a file, which has some impact in play. For example, a video editing software installer has its files compressed beforehand, which would ``reduce the bandwidth required`` when downloading it and result in a ``shorter transmission time``. When the user has finished downloading, it would also benefit them by ``reducing the storage space required`` to store the installer.