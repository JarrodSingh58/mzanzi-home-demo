# Mzansi Home

A small standalone budgeting app for low-income South African households.

## Why it exists

Many households work with very little money and no easy way to see what is left each day after rent, food, electricity and other bills. Mzansi Home answers one question clearly: how much can each person in the house spend today?

## What it does

- Shows a headline figure: what is left per person per day this month
- Tracks income and spending for Rent, Food, Electricity, Transport, School and Savings
- Lets you set a share of your income for each area and shows spent against allocated
- Tracks things you own and things you owe, with your net worth
- Profit and Loss and Balance Sheet reports for this month, last month, this year or a custom period, with a print or PDF export
- Short, plain advice for each area, written for South Africa
- Demo data that can be reset at any time

## How to use it

1. Open `index.html` in any modern browser. An internet connection is needed once to load the Pico CSS styles.
2. Log in with username `demo` and password `demo`.
3. Use the month and year at the top to move between months.
4. Pick a tab, set an allocation and save entries as you spend.
5. Open Settings and choose Reset data to restore the demo data.

## Privacy

Everything is stored in your browser on your own device. Nothing is sent to a server, and there are no accounts, analytics or tracking. The demo login is only a screen and is not real security.

## How it is built

One `index.html` file with vanilla JavaScript and no build step, styled with Pico CSS from a CDN plus a small style block. Data is kept in localStorage.

## Keeping token use low

- The whole app lives in a single HTML file, so there is only one file to generate, read and edit.
- It was built from one prompt that held all the key information and details up front, so there was little back and forth.
- The prompt was specific about layout, behaviour and data, which avoided rework and extra tokens.

## Limitations

- It is a demo, so the login is not secure
- Data lives only in one browser on one device, so clearing browser data removes it
- No sync between devices and no backup or import
- Amounts are in rand and the app is in English only
- The advice is general information and not financial or legal advice
