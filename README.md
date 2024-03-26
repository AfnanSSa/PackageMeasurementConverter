The input strings represent measurement packages and follow a specific encoding format. Each package consists of a number indicating the count of values measured in each measurement cycle, followed by the measured values.
The values are encoded using alphabetical characters, with "a" representing 1, "b" representing 2, and so on, up to "z" representing 26.
Numbers higher than 26 are encoded with multiple characters that are added
together. The encoding format is terminated with the first non-"z" character
following a sequence of multiple characters representing a number.

input=aa -> [1]
input-abbcc -> [2, 6]
input=dz_a_aazzaaa -> [28, 53, 1]
