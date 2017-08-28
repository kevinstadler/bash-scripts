#!/bin/sh
pandoc "$1" --filter pandoc-citeproc -o "`basename "$1" .md`.pdf"
