---
title: Uploading files
sidebar_label: Uploading files
---

In self-service solutions, there is often a need to upload documentation in the form of documents. HOw to make sure that these documents do not contain anything malicious? 

## File type verification
You can't trust filename extensions(DOC, PDF, Etc.) to tell the truth about what type of file you are receiving. A simple and more secure way of verifying what type of file you are dealing with is to check the file's signature (not to be confused with a cryptographic signature), somtimes referred to as a "magic numbers" or "magic bytes". On the command line you can do this with the command [file](https://linux.die.net/man/1/file), in the code you have to do it yourself. A valid PDF file, for example, always start with the sequence ```25 50 44 46 2D```. More about these sequences can be found [List of file signatures](https://en.wikipedia.org/wiki/List_of_file_signatures)

## Encryption 
needs to be written