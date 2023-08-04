# Wrangler minimal reproduction for #2978

1. Copy both `wrangler.toml.example` -> `wrangler.toml` with correct account ID in both `apps\worker-a` and `apps\worker-b`
2. `npm install`
3. `npm run dev`

## Expected result

Should work

## Actual result

If wrangler hasn't been used recently, it fails the first time with this error:

`✘ [ERROR] You must be logged in to use wrangler dev in remote mode. Try logging in, or run wrangler dev --local.`

And then it works 2nd run.
