# Solid State Physics: crystals, defects and bands

A cleaned-up, illustrated study note rebuilt from the handwritten class notes (Yeasir Sir). Items marked added were missing from the original and fill a gap.

## Learning roadmap: study in this order

1. [Crystalline vs amorphous solids](#s1)Why order matters: long-range vs short-range.
2. [Lattice, basis and unit cell](#s2)The vocabulary everything else depends on.
3. [Crystal systems](#s3)Cubic and hexagonal (plus the full list of 7).
4. [Cubic system: SC, BCC, FCC](#s4)Where the atoms sit, coordination number.
5. [Counting atoms per unit cell](#s5)Corner = 1/8, face = 1/2, body = 1.
6. [Packing fraction](#s6)Geometry, derivations, and why FCC > BCC > SC.
7. [Miller indices](#s7)Naming planes with three numbers.
8. [Single crystal vs polycrystal](#s8)Grains and grain boundaries.
9. [Crystal defects](#s9)Point, line, plane; Frenkel and Schottky.
10. [Band theory of solids](#s10)From atomic levels to energy bands (Si example).
11. [Worked problem: KCl lattice constant](#s11)Density, mass of unit cell, lattice constant.
12. [Check before the exam](#s12)Small slips and gaps found in the original note.

## 1Crystalline vs amorphous solids

Solids fall into two families, depending on how regularly their atoms are arranged.

| Type | Order | Meaning |
| --- | --- | --- |
| Crystalline | Long-range order | The pattern repeats across the whole solid. |
| Amorphous | Short-range order | Only the nearest neighbours follow a pattern; it fades with distance. |

Crystalline: every atom sits on a repeating grid

Amorphous: neighbours are close, but the grid is lost

## 2Lattice, basis and unit cell

**Crystal structure** = lattice + basis

- **Lattice:** an endless array of points that repeats in space.
- **Basis:** the atom (or group of atoms) attached to every lattice point.
- **Unit cell:** the small building block that, repeated in all directions, builds the whole crystal.
- **Primitive cell:** a unit cell with lattice points only at its corners.
- **Centered cells:** unit cells with extra lattice points at the *body* centre, the *face* centres, or the *base* faces.

Place the same basis on every lattice point and you get the crystal

## 3Crystal systems

Crystals are grouped by the lengths (a, b, c) and angles (α, β, γ) of the unit cell. The note covers two of them in detail:

| System | Edge lengths | Angles |
| --- | --- | --- |
| Cubic | a = b = c | α = β = γ = 90° |
| Hexagonal | a = b ≠ c | α = β = 90°, γ = 120° |

Base of the hexagonal cell: two equal edges at 120°

### All seven systems added

The note says there are 7 types but lists two. For completeness:

| System | Edges | Angles |
| --- | --- | --- |
| Cubic | a = b = c | α = β = γ = 90° |
| Tetragonal | a = b ≠ c | α = β = γ = 90° |
| Orthorhombic | a ≠ b ≠ c | α = β = γ = 90° |
| Hexagonal | a = b ≠ c | α = β = 90°, γ = 120° |
| Trigonal (rhombohedral) | a = b = c | α = β = γ ≠ 90° |
| Monoclinic | a ≠ b ≠ c | α = γ = 90° ≠ β |
| Triclinic | a ≠ b ≠ c | α ≠ β ≠ γ |

## 4Cubic system: SC, BCC, FCC

The cubic system has three common unit cells. In the drawings, **blue** atoms are at corners, **orange** at the body centre, and **green** at face centres.

**Simple cubic (SC)**\
corners only

**Body-centred (BCC)**\
corners + body centre

**Face-centred (FCC)**\
corners + face centres

| Cell | Atoms per cell | Coordination number | Touching atoms give | Packing |
| --- | --- | --- | --- | --- |
| SC | 1 | 6 | a = 2r | ≈ 52% |
| BCC | 2 | 8 | √3·a = 4r | ≈ 68% |
| FCC | 4 | 12 | √2·a = 4r | ≈ 74% |

**Coordination number (CN)** = how many nearest neighbours one atom touches.

## 5Counting atoms per unit cell

An atom on a cell corner or face is shared with neighbouring cells, so only a fraction of it belongs to this cell.

| Position | Shared by | Share inside one cell |
| --- | --- | --- |
| Corner (8 per cell) | 8 cells | 1/8 |
| Face centre (6 per cell) | 2 cells | 1/2 |
| Body centre (1 per cell) | 1 cell | 1 |

SC: 8 × 1/8 = **1**\
BCC: 8 × 1/8 + 1 = **2**\
FCC: 8 × 1/8 + 6 × 1/2 = 1 + 3 = **4**

## 6Packing fraction

How much of the unit cell is actually filled by atoms (treated as touching hard spheres of radius r).

Packing fraction = (volume of atoms in the cell) ÷ (volume of the cell)\
= (n × 4/3 π r³) ÷ a³ where n = atoms per cell

### Step 1: find a in terms of r (where atoms touch)

**SC:** atoms touch along the edge\
a = 2r

**BCC:** atoms touch along the body diagonal (cut plane shown)\
√3·a = 4r, so a = 4r/√3

**FCC:** atoms touch along the face diagonal\
√2·a = 4r, so a = 4r/√2

Why 4r? Along each diagonal, you pass through half an atom, a whole atom, and half an atom on each side of the centre: that is r + 2r + r = 4r.

### Step 2: substitute

**SC** (n = 1, a = 2r)

PF = (4/3 π r³) ÷ (2r)³ = (4/3 π r³) ÷ 8r³ = π/6 = 0.5236 → **52.36%**\
The remaining ≈ 47.6% of the cell is empty space.

**BCC** (n = 2, a = 4r/√3)

PF = 2 × (4/3 π r³) ÷ (4r/√3)³ = (8/3 π r³) ÷ (64r³ / 3√3) = π√3/8 = 0.6802 → **≈ 68.0%**

**FCC** (n = 4, a = 4r/√2 = 2√2·r)

PF = 4 × (4/3 π r³) ÷ (2√2·r)³ = (16/3 π r³) ÷ (16√2·r³) = π/(3√2) = 0.7405 → **≈ 74.0%**

Packing fraction compared

**Order to remember:** FCC (74%) > BCC (68%) > SC (52%). More atoms per cell and more touching neighbours (CN 12 > 8 > 6) means tighter packing.

## 7Miller indices

Miller indices (h k l) name a plane in a crystal using three small integers.

### Three steps

1. **Intercepts:** note where the plane cuts the x, y and z axes (in units of the cell edge). If the plane runs parallel to an axis, that intercept is ∞.
2. **Reciprocals:** invert each intercept (1/∞ = 0).
3. **Clear fractions:** multiply by the smallest number that turns them all into whole numbers.

| Example from the note | x | y | z |
| --- | --- | --- | --- |
| 1. Intercepts | 1 | 2 | 1 |
| 2. Reciprocals | 1 | 1/2 | 1 |
| 3. Multiply by 2 | 2 | 1 | 2 |

Result: the plane is written **(2 1 2)**

### Planes of the cube

Axes: x points right, y goes back into the page, z points up. The shaded area is the plane.

**(1 0 0)**\
cuts x at 1, parallel to y and z

**(0 1 0)**\
cuts y at 1, parallel to x and z

**(0 0 1)**\
cuts z at 1, parallel to x and y

**(1 1 0)**\
cuts x and y at 1, parallel to z

**(1 0 1)**\
cuts x and z at 1, parallel to y

**(1 1 1)**\
cuts all three axes at 1

## 8Single crystal vs polycrystal

- **Single crystal:** one continuous lattice, same orientation everywhere.
- **Polycrystal:** many small crystals called **grains**, each with its own orientation. A grain is a single crystal sitting inside the polycrystal.
- The surfaces where grains meet are **grain boundaries**.

Single crystal: all arrows (lattice directions) agree

Polycrystal: four grains, four orientations

## 9Crystal defects

Real crystals are never perfect. Defects are grouped by their dimension:

| Class | Dimension | Examples |
| --- | --- | --- |
| Point defect | 0-D (one site) | Frenkel, Schottky |
| Line defect | 1-D | Dislocations added |
| Plane defect | 2-D | Grain boundaries added |

**Frenkel defect:** an atom leaves its site (vacancy, dashed) and squeezes into an interstitial position

**Schottky defect:** atoms leave the crystal completely, leaving vacancies (dashed)

|  | Frenkel | Schottky |
| --- | --- | --- |
| What happens | Atom moves to an interstitial position inside the crystal | Atoms leave the lattice and the crystal |
| Density | **Stays the same** (nothing is lost) | **Decreases** (mass is lost, volume is not) |

**Memory hook:** Frenkel = the atom *moves*, so density is unchanged. Schottky = the atom *leaves*, so density drops.

In ionic crystals, a Schottky defect is usually a missing cation–anion *pair* (that is why two vacancies are drawn). added

## 10Band theory of solids

### Starting point: electrons in one atom

An isolated atom has sharp, separate energy levels. For silicon (atomic number 14):

Si (14) = 1s² 2s² 2p⁶ 3s² 3p²

The levels are labelled 1st, 2nd, 3rd going up in energy.

### From levels to bands

A single-crystal piece of silicon contains an enormous number of atoms (the note writes \~10²⁴). Their levels cannot all stay at the same energy, so each level splits into a huge number of very closely spaced levels. Together they form an **energy band**: a band of energy.

Each atomic level broadens into a band when many atoms form a crystal

### What comes next added

The note stops here. The next ideas in this chapter are the **valence band** (highest filled band), the **conduction band** (empty band above it) and the **band gap** between them. A small gap gives semiconductors like Si, a huge gap gives insulators, and overlapping bands give metals.

## 11Worked problem: KCl lattice constant

**Problem.** The density of a KCl crystal is 1.98 × 10³ kg/m³. Find the lattice constant and the distance between two adjacent atoms. The lattice is face-centred cubic (FCC).

1. **Mass of one formula unit.** Molar mass = 39 + 35.5 = 74.5 g/mol. One KCl unit weighs 74.5 ÷ (6.023 × 10²³) g.
2. **Mass of the unit cell.** An FCC cell holds 4 KCl units:

   m = 4 × 74.5 ÷ (6.023 × 10²³) g = 4.95 × 10⁻²² g = **4.95 × 10⁻²⁵ kg**
3. **Lattice constant.** Density = mass ÷ volume = m ÷ a³, so

   a = (m/ρ)1/3 = (4.95 × 10⁻²⁵ ÷ 1.98 × 10³)1/3 = (2.50 × 10⁻²⁸)1/3 ≈ 6.3 × 10⁻¹⁰ m = **6.3 Å**
4. **Distance between adjacent atoms** completed. In KCl, a K⁺ and a Cl⁻ sit next to each other along the cell edge, so

   d = a/2 ≈ **3.15 Å**

   Two atoms of the same kind (K–K) are nearest along a face diagonal: a/√2 ≈ 4.45 Å.

One edge of the cell: K⁺ and Cl⁻ alternate, so neighbours are a/2 apart

## 12Check before the exam

**Small things to fix in the original note**

- **FCC atom count (pink margin note):** it reads "corner + body centre". FCC is corner + **face** centres: 1 + 6×1/2 = 4. Body-centre belongs to BCC.
- **Rounding:** BCC packing is π√3/8 = 0.6802 (68.02%), the note has 68.01%. FCC is 0.7405 (74.05%), the note has 74.04%. Either is fine at 2 decimals if you state "≈".
- **KCl mass:** 4 × 74.5 ÷ 6.023×10²³ = 4.95×10⁻²⁵ kg, not 4.92×10⁻²⁵. The final a ≈ 6.3 Å is unaffected.
- **KCl problem:** the "distance between adjacent atoms" part was left unfinished; the answer is a/2 ≈ 3.15 Å.
- **Coordination number of FCC:** the note line is cut off; it is 12.

**Quick self-test**

1. Why does a Schottky defect lower density while Frenkel does not?
2. Derive the SC packing fraction from a = 2r without looking.
3. Find the Miller indices of a plane with intercepts (2, 1, ∞).
4. What is the relation between a and r for BCC, and why?

Built from the handwritten solid state physics notes. Bengali margin remarks in the original (e.g. "atom ফাঁকা", "density ... আগের মতো") are folded into the explanations above.