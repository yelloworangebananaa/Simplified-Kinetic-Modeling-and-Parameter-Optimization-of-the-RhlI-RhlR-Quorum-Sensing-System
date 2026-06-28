# Simplified-Kinetic-Modeling-and-Parameter-Optimization-of-the-RhlI-RhlR-Quorum-Sensing-System
for more information go to: cellsandcivics.org

Methodology

The model was implemented in Tellurium using a reaction based framework consisting of four molecular species:

RhII

C4-HSL

RhlR

Complex

The simulation was initialized with the following concentrations:

RhII = 0.05

C4-HSL = 0

RhlR = 1.0

Complex = 0

A central feature of the model was the inclusion of a Hill function within the RhII production equation:

RhII Production = rhli_basal + rhli_act × (Complexⁿ / (Kⁿ + Complexⁿ))

where:

K = 0.4

n = 3

The Hill function introduces nonlinear activation into the system. When complex concentration is low relative to K, the activation term remains small. As complex concentration approaches K, the activation term increases more rapidly. Because n = 3, the response becomes steeper than a simple linear relationship, creating a threshold-like transition between low and high activation states.

Additional reactions included C4-HSL production by RhII, reversible binding between C4-HSL and RhlR to form the complex, and degradation pathways for RhII and C4-HSL. The simulation was run from 0 to 200 time units with 1000 computational steps.
