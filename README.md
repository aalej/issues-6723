# Repro for issue 6723

## Setup

platform: Windows 10, macOs 14.2.1<br>
firebase-tools: v13.1.0<br>
node: v18.16.1

## Steps to reproduce

1. Install dependencies
   - Run `cd functions` and `npm i`
   - Install jest `npm i -g jest`
1. Run `npm run build`
1. Run `firebase emulators:exec "jest --coverage" --project <project_id>`
   - Tests is located in `functions` folder
