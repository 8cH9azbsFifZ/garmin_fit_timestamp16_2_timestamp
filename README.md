# garmin_fit_timestamp16_2_timestamp
Convert the timestamp_16 field of .FIT files to timestamp. The timestamp_16
fields are relative timestamps. This script will calculate an absolute 
timestamp and add it to the data file.

# Installation
OSX

    # brew install gawk jq

Debian

    # apt-get -y install gawk jq


# Using

1. Convert .fit file to .json, i.e. using [Garmin-FIT](https://github.com/mrihtar/Garmin-FIT).
2. Add the new absolute timestamp using `cat infile.json |./garmin_timestamp16_to_timestamp > outfile.json`.
