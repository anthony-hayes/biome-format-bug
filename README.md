# biome-format-bug

REPRODUCTION

1. Run `biome format .` using `npm run format`

EXPECTED:

only the files in `pk1/pk1-1` should be formatted

ACTUAL:

Only files in the root of the project are looked at.
Changing the command to `biome format ./**/*` will look at more files, but error on a large project "spawn E2BIG"
