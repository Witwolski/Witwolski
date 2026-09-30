# Lesson 1: Charge, Current, Voltage, Resistance and Ohm's Law

**Why this matters for control systems:** a control system *measures* something (with a sensor), *decides* what to do (with a controller), and *acts* (by sending electricity to a motor, heater or valve). All three depend on the four ideas in this lesson.

---

## 1. Charge

Everything is made of atoms. Atoms contain tiny particles called **electrons**, and each electron carries a small amount of **electric charge**.

In metals like copper, some electrons can move freely through the material. Moving charge is what electricity is.

- Symbol: **Q**
- Unit: **coulomb (C)**
- 1 coulomb is the charge of about 6.24 × 10¹⁸ electrons. One electron carries a very small amount of charge, so a huge number is needed to make 1 coulomb.

---

## 2. Current

**Current** is how much charge flows past a point in a wire each second.

- Symbol: **I**
- Unit: **ampere, or "amp" (A)**
- **1 amp = 1 coulomb of charge passing a point every second**

More charge passing each second means a bigger current.

**Direction:** on circuit diagrams, current is drawn flowing from the **positive (+)** side of the battery to the **negative (−)** side. This is called **conventional current**. Electrons actually move the opposite way, but the + to − convention was chosen before electrons were discovered and it has stuck. It doesn't change any calculations, so always use + to −.

---

## 3. Voltage

**Voltage** is what pushes current around a circuit. A battery or power supply provides this push.

- Symbol: **V**
- Unit: **volt (V)**
- Exact meaning: **1 volt = 1 joule of energy given to each coulomb of charge**. A higher voltage gives each bit of charge more energy.

**Key point: voltage is always measured *between two points*.** That's why it's also called **potential difference**. A 9 V battery has 9 volts *between its two terminals*. It's also why a multimeter uses **two** probes to measure voltage.

When someone says "this point is at 5 V", they mean 5 V *compared with a reference point*. That reference point is called **ground** or **0 V**.

---

## 4. Resistance

**Resistance** is how strongly something opposes the flow of current.

- Symbol: **R**
- Unit: **ohm (Ω)**

- **Low resistance:** current flows easily. Copper wire is an example.
- **High resistance:** very little current flows. Rubber and plastic are examples, which is why they're used to insulate wires.

A **resistor** is a component made to have a specific resistance. Engineers use resistors to control how much current flows.

When current flows through a resistance, some electrical energy turns into **heat**. Kettles and toasters work this way, and it's also why overloaded wires can overheat.

---

## 5. Ohm's Law

Voltage, current and resistance are linked by one equation:

$$
V = I \times R
$$

**Voltage = Current × Resistance**

You can rearrange it depending on what you need to find:

| To find | Use |
|---|---|
| Voltage | V = I × R |
| Current | I = V ÷ R |
| Resistance | R = V ÷ I |

What **I = V ÷ R** tells you:
- **More voltage, same resistance:** more current.
- **More resistance, same voltage:** less current.
- **Double the resistance:** the current halves.

**Memory trick:** draw a triangle with V on top and I and R underneath.
```
      V
   -------
    I | R
```
Cover the letter you want to find, and what's left shows the formula. Cover V to get I × R. Cover I to get V ÷ R. Cover R to get V ÷ I.

### Worked examples

**Example 1.** A 12 V battery is connected across a 6 Ω resistor. What current flows?
I = V ÷ R = 12 ÷ 6 = **2 A**

**Example 2.** A current of 0.5 A flows through a 20 Ω resistor. What is the voltage across it?
V = I × R = 0.5 × 20 = **10 V**

**Example 3.** A 24 V supply pushes 3 A through a heater. What is the heater's resistance?
R = V ÷ I = 24 ÷ 3 = **8 Ω**

(24 V is worth remembering. It's the standard voltage used in most industrial control panels.)

---

## 6. Circuits: current needs a complete loop

Current only flows if there is a **complete loop** from the + side of the source, through the components, and back to the − side. This loop is called a **circuit**.

| Situation | What it means | Resistance | Current |
|---|---|---|---|
| **Closed circuit** | Complete loop, working normally | Normal | Set by Ohm's law |
| **Open circuit** | The loop is broken, e.g. a switch is off, a wire is cut, or a fuse has blown | Effectively infinite | **Zero** |
| **Short circuit** | Current finds a path with almost no resistance and skips the normal load | Nearly zero | **Very large**. Dangerous: it causes heat, fire and blown fuses |

**Important:** you can have voltage without any current. A battery sitting on a shelf has voltage between its terminals, but no current flows because there's no complete loop. Current, however, cannot flow without a voltage to push it.

**Why short circuits are dangerous:** Ohm's law says I = V ÷ R. If R is almost zero, I becomes very large. **Fuses** and **circuit breakers** are there to cut off the current before that causes damage.

---

## Summary

| Quantity | Symbol | Unit | Meaning |
|---|---|---|---|
| Charge | Q | coulomb (C) | An amount of electricity |
| Current | I | amp (A) | How much charge flows per second |
| Voltage | V | volt (V) | The push that drives current, always measured between two points |
| Resistance | R | ohm (Ω) | How strongly something opposes current |

**Ohm's Law: V = I × R**

---

## Quick self-check

1. If you double the voltage and keep the resistance the same, what happens to the current?
2. Can a circuit have voltage but no current? Give an example.
3. A 9 V battery is connected to a 3 Ω resistor. What current flows?

<details>
<summary>Answers (try first)</summary>

1. The current **doubles**, because I = V ÷ R.
2. **Yes.** A battery with nothing connected to it, or a circuit with its switch off. The voltage is there, but there's no complete loop.
3. I = 9 ÷ 3 = **3 A**.

</details>

---

**Your first test arrives tomorrow at 7pm (Brisbane time).**
