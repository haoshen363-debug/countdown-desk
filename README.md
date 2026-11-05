# Countdown Desk

A small, offline countdown page. Set a name and a target date, and keep the remaining days, hours, minutes, and seconds on your desk.

## Use

Download this repository and open `index.html` in a modern browser. No build step, package installation, or account is required.

- Choose a date in your computer's local time zone.
- Use the one-hour and one-day shortcuts for quick timers.
- Your target is saved in this browser's local storage when available.
- Clear removes this application's saved target.
- A reached deadline stays at zero. There are no background notifications after the page is closed.

The interface is in Simplified Chinese. All project files use UTF-8.

## Privacy

The page makes no network requests and uses no analytics, external fonts, cookies, or third-party scripts. It only stores your target and its label in local storage under `countdown-desk:v1`.

## Development

Edit `index.html` and reload it. The timer uses the current system clock rather than decrementing a counter, so a sleeping or background tab catches up when it resumes.

To serve it locally instead of opening the file directly:

```sh
python -m http.server 8080
```

Then visit `http://localhost:8080`. Opening the HTML file directly may have different local-storage behavior across browsers.

## License

MIT. See [LICENSE](LICENSE).
