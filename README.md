# Frame Tuner for Windows — Lower Input Lag, Smooth Out Stutters

A small Windows utility that tunes the system for low input lag and steady frame delivery. It flips a handful of OS switches that benefit real-time, interactive workloads — timer resolution, GPU scheduling, power plan, background services — and gives you a one-click **Restore Defaults** so nothing sticks around after you quit. Free, portable, no account, no watermark, no ads.

![Frame Tuner for Windows — low input lag, smooth frame delivery](screenshot.png)

The app does not overclock, does not touch registry outside its own named keys, and does not install any driver.

## Download

**Latest build:** [BloxBoost.zip](../../releases/latest/download/BloxBoost.zip)

Self-contained archive. Unzip anywhere, run the app from the folder. No installer, no admin prompt beyond the one Windows itself shows for timer-resolution tweaks.

## Features

- **Timer resolution** — temporarily drops the system timer resolution to 0.5 ms for the running session, reducing frame-pacing variance in interactive apps.
- **GPU scheduling** — toggles Windows Hardware-Accelerated GPU Scheduling (HAGS) if the driver supports it.
- **High-performance power plan** — switches the active plan, remembers the previous one, restores on exit.
- **Background slimming** — pauses non-essential background services for the session (Search indexer, delivery optimisation, scheduled telemetry).
- **One-click Restore Defaults** — rolls back every change, re-enables what was paused, returns the power plan.
- **Portable** — no registry footprint outside the app's own named keys, no scheduled tasks, no services installed.
- **Offline** — the app does not make a single network call after unzip.

## How to use

1. Launch the app from the unzipped folder.
2. Press **Apply** to turn on the tuning set.
3. Do whatever you came to do.
4. Press **Restore Defaults** (or close the app) to roll everything back.

## FAQ

**Is it really free?**
Yes. Free forever, MIT licensed.

**Does it need admin?**
Timer-resolution tweaks need admin, Windows shows the standard UAC prompt once per launch. Nothing else is elevated.

**Does it leave anything behind after I close it?**
No. Timer resolution is session-scoped; power plan and background services are restored on exit.

**Does it work on Windows 11?**
Yes. Windows 10 and Windows 11, 64-bit.

## System requirements

- Windows 10 or Windows 11, 64-bit

## License

MIT.
