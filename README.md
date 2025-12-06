# aya_ha_debugger

`aya_ha_debugger` is a cheeky upgrade from the tired `print()` statements we scatter through code just to make sure our logic ran. Instead of dreaming up yet another “made it here” string, you call `aya_ha()` and it shouts the signature message for you—no thinking, no typing, no boredom.

## Why not print?
- Boring strings slow you down and clutter diffs.
- You forget to change the text, so every log looks the same.
- Debugging should feel fun (or at least painless).

`aya_ha()` fixes that by emitting a bold banner so you can spot the execution path instantly. Want more context? Pass a short description and it folds it into the same banner.

## Usage
```python
from aya_ha_debugger import aya_ha

# Zero-config: just make sure the code path ran.
aya_ha()
# ***** aya ha *****

# Add context when you need it.
aya_ha("first if condition")
# ***** first if condition me aya ha *****
```

## Installation
```bash
pip install aya_ha_debugger
```

Embrace the modern, drop the manual `print()`, and let `aya_ha()` tell you exactly where the code went.
