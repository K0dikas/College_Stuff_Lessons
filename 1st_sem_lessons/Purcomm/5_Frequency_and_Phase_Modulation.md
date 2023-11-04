- **Frequency Modulation** `FM` - A *modulation process* that puts the message in a `carrier wave` by changing the *instantaneous frequency* of the wave. 
- **Characteristics: **
	- The carrier frequency shifts proportionately as the modulating signal's amplitude varies.
	- The carrier frequency increases as the modulating signal amplitude increases.
	- If a reverse relationship is implemented, a decreasing modulating signal will increase the carrier frequency above its center value, while an increasing modulating signal will decrease the carrier frequency below the center value.

- **Frequency Deviation** - It is the *amount of change* in the *carrier frequency* caused by the *modulating signal*. The *maximum frequency* deviation happens at the *maximum amplitude* of the modulating signal.
	- `FORMULA`
		*Maximum Deviation* = `Carrier frequency` *+* `Maximum Frequency`
		*Minimum Deviation* = `Carrier frequency` *-* `Maximum Frequency`
		*fd* = `Maximum deviation` *-* `Minimum deviation`
	- **Note:** To convert `kHz` to `MHz`, *divide* `kHz` by `1000`

- **Frequency-shift Keying** `FSK` - In `FM`, a series of *rectangular waves*, such as *serial binary data*, can present the *modulating signal*. This kind of *modulating signal* will only have `two amplitudes` and will also make the *carrier frequency* have `two values` `(1 and 0)`, such as this *modulating signal*
	- `Binary 0` *=>* *Wide wavelength*
	- `Binary 1` *=>* *Narrow wavelength*

- **Phase Modulation** `PM` - A *modulation process* wherein the phase of the carrier signal varies based on the *amplitude variation* of the *message signal* or *modulating signal*.
	- `Lagging phase shifts` and `Leading phase shifts` - the *frequency* `compresses` in accordance with the positive *modulating signal* while it stretches when at zero deviation.

- **Phase-shift Keying** `PSK` - In `PM`, the *modulating signal* can also be used with the *binary signal*. When the *binary* `0` is `0`*V*, when the `PM` *signal* is simply the *carrier frequency*, and when a *binary* `1` voltage level occurs `(3V)`, the *modulator*, or *phase shifter*, changes the phase of the carrier, and not its *frequency*.
	- `Binary 0` *=>* *Wide Wavelength*
	- `Binary 1` *=>* *Upside-down mcdo || 180 phase shifts*
		- This *process* is called `phase-shift keying` or `binary phase-shift keying`

##### Sidebands and Modulation Index (Frenzel, 2022)
-  When a `constant-frequency sine wave` *modulates a carrier* , two side frequencies or *sidebands* are produced. In `FM` and `PM`, just like with **Amplitude Modulation** `AM`, it is the *sum* and *difference* of the carrier and the *modulating frequency*. The spectrum of an `FM` and a `PM` *signal* is wider than `AM` because of *sideband pairs*.

- **Modulation Index** - The *amplitudes* of the `carrier` and `sidebands of the frequency spectrum` of an `FM` signal still depend on the *modulation index* `mf` still unitless.

- **Bessel Functions** - The `number` and `amplitudes` of the *sidebands* are obtained by solving the `FM` signal equation.