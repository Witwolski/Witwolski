# Lesson 1: Charge, Current, Voltage, Resistance and Ohm's Law

**Why this matters for control systems:** a control system does three things. It *measures* (sensors, which usually output a voltage or current), it *decides* (a controller such as a PLC), and it *acts* (it sends current to motors, heaters and valves). All three run on the four ideas in this lesson. Master these and everything after builds on them.

---

## 1. Charge: the players

Everything is made of atoms, and atoms contain tiny particles called **electrons** that carry a negative **electric charge**. In a metal wire, some electrons are loosely held and can move around.

- Symbol: **Q**
- Unit: **coulomb (C)**
- 1 coulomb is the charge of about **6.24 × 10¹⁸ electrons** (6.24 billion billion).

🏉 **Analogy:** charge is the **players on the field**. On their own, standing still, they do nothing. Things only get interesting when they move.

---

## 2. Current: how many players cross the gain line per second

**Current** is the *flow* of charge: how much charge passes a point in the wire every second.

- Symbol: **I** (from the French *intensité*)
- Unit: **ampere, or "amp" (A)**
- **1 amp = 1 coulomb passing a point per second**

🏉 **Analogy:** stand on the **gain line** and count how many players surge across it each second. Lots of players crossing each second is a high current. A trickle is a low current.

Key point: current is measured **at a point**, like counting at one line on the field. The same current flows *through* a component.

> ⚠️ **Where the analogy breaks:** electrons in a wire actually drift very slowly, only millimetres per second. But they're packed shoulder to shoulder all the way around the circuit, so when you flip a switch they *all* start moving almost instantly. Think of a scrum where the whole pack moves together, not one runner sprinting the length of the field.

> 📝 **A quirk you need to know:** engineers draw current flowing from **+ to −**. This is called **conventional current**. Electrons actually move the other way, from − to +. The convention was set before electrons were discovered, and it stuck. For circuit calculations the direction choice doesn't change any answers. Just use conventional current (+ → −) like every schematic does.

---

## 3. Voltage: the shove from the pack

**Voltage** is the "push" that drives charge around a circuit. More precisely, it's the **energy given to each coulomb of charge**.

- Symbol: **V** (sometimes **U** or **E** in textbooks)
- Unit: **volt (V)**
- **1 volt = 1 joule of energy per coulomb**

🏉 **Analogy:** voltage is **the drive of the forward pack in a scrum**. A battery is like the pack: it provides the shove. A 12 V battery shoves harder than a 1.5 V AA battery.

### The most important thing about voltage: it's always *between two points*

Voltage is also called **potential difference**. It only makes sense as a comparison between two points, just as *field position* only makes sense relative to something ("we're 10 metres from their try line").

🏉 Picture a **field on a slope**. What makes a ball roll isn't how high the field is above sea level, it's the **height difference** between one end and the other. Voltage works the same way: it's the "height difference" in electrical energy between two points. That's why a multimeter has **two** probes when measuring voltage.

When someone says "this point is at 5 volts", they mean *5 volts relative to a reference point*, usually called **ground** or **0 V**. Ground is like your own try line: the point you measure everything from.

---

## 4. Resistance: the defensive line

**Resistance** is how much a material *opposes* the flow of current.

- Symbol: **R**
- Unit: **ohm (Ω)**

🏉 **Analogy:** resistance is **the opposition's defensive line**.
- A weak, rushed defence (**low resistance**): your players pour through, so lots of current.
- A brick-wall goal-line stand (**high resistance**): barely anyone gets through, so little current.

Copper wire has very low resistance. That's why wires are made of it. Rubber and plastic have extremely high resistance, which is why they're used as insulation. **Resistors** are components made to have a specific resistance, so engineers can control how much current flows.

> ⚠️ **Where the analogy breaks:** when current pushes through a resistance, energy is turned into **heat**. That's how toasters and kettles work, and why overloaded wires can start fires. A defensive line doesn't literally heat up, although if you've ever been at the bottom of a ruck you might disagree.

---

## 5. Ohm's Law: the relationship between them all

These three quantities are linked by one of the most-used equations in all of engineering:

$$
V = I \times R
$$

**Voltage = Current × Resistance**

Rearranged, depending on what you need:

| Want to find | Formula |
|---|---|
| Voltage | V = I × R |
| Current | I = V ÷ R |
| Resistance | R = V ÷ I |

🏉 **Reading it as rugby:** **I = V ÷ R** says:
- **Harder shove (more V), same defence:** more players get across the line (more I).
- **Stronger defence (more R), same shove:** fewer get across (less I).
- **Double the defence, same shove:** half as many get through.

### Memory trick: the triangle
```
      V
   -------
    I | R
```
Cover the one you want. Cover **V** and you see **I × R**. Cover **I** and you see **V over R**. Cover **R** and you see **V over I**.

### Worked examples

**Example 1.** A 12 V battery is connected across a 6 Ω resistor. What current flows?
I = V ÷ R = 12 ÷ 6 = **2 A**

**Example 2.** 0.5 A flows through a 20 Ω resistor. What's the voltage across it?
V = I × R = 0.5 × 20 = **10 V**

**Example 3.** A 24 V supply pushes 3 A through a heater. What's the heater's resistance?
R = V ÷ I = 24 ÷ 3 = **8 Ω**

> 24 V comes up a lot in your future career: it's the standard control voltage in most industrial control panels.

---

## 6. The circuit: you need a complete loop

Current only flows around a **complete loop**, called a **circuit**. It goes out of the source, through the components, and back into the source.

🏉 **Analogy:** think of a set play that has to go all the way around and come back to the start. Break the chain anywhere and the whole play stops.

Three situations to know:

| Situation | What it is | Resistance | Current |
|---|---|---|---|
| **Closed circuit** | Complete loop, working normally | Normal | Normal, set by Ohm's law |
| **Open circuit** | Loop broken: switch off, wire cut, blown fuse | Effectively infinite | **Zero** |
| **Short circuit** | Current finds a path with almost no resistance, bypassing the load | Nearly zero | **Huge**. Dangerous: heat, fire, blown fuses |

🏉 **Open circuit:** an **unbreakable wall** across the field. The pack still shoves as hard as ever (the **voltage is still there**), but **nobody gets through (zero current)**.

> 💡 This is a classic trap question: **you can have voltage without current.** A battery sitting on a shelf has 1.5 V across its terminals but no current flows, because there's no loop. Current, on the other hand, needs voltage to push it.

🏉 **Short circuit:** the defence walks off the field. With almost nothing in the way, current becomes enormous. Ohm's law shows why: I = V ÷ R, and when R is tiny, I is huge. That's why we have **fuses and circuit breakers**. They're the referee who blows the whistle and stops play before someone gets hurt.

---

## Summary card

| Quantity | Symbol | Unit | Rugby picture |
|---|---|---|---|
| Charge | Q | coulomb (C) | The players |
| Current | I | amp (A) | Players crossing the gain line per second |
| Voltage | V | volt (V) | The pack's shove, always measured between two points |
| Resistance | R | ohm (Ω) | The defensive line |

**Ohm's Law: V = I × R**

---

## Quick self-check (no marks, just see if it stuck)

1. If you double the voltage and keep the resistance the same, what happens to the current?
2. Can a circuit have voltage but no current? Give an example.
3. A 9 V battery is connected to a 3 Ω resistor. What current flows?

<details>
<summary>Answers (only click after you've tried)</summary>

1. The current **doubles** (I = V ÷ R, so V up ×2 means I up ×2).
2. **Yes.** A battery with nothing connected, or an open switch. The voltage is there but there's no complete loop.
3. I = 9 ÷ 3 = **3 A**.

</details>

---

**Your first real test arrives tomorrow at 7pm (Brisbane time).**
