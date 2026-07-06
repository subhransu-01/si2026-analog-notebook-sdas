<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A01`

**Status:** ❌ Not approved

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **1.25 column H avg; min 1; max 1.5**

### Reviewer remarks
- Very ambitious project and total area may not be permissible.
- 5 GHz LC VCO: LC tank or ring-oscilattor ? either ways it is going to be very challenging.
- The block "linear gain" is a power amplifier, another ambitious project.
- Suggestion: pick a small subsystem like the I-Q modulator or
- A PLL with low-frequrncy (< 1GHz) ring-oscillator as VC
- It is an interesting proposal, however, it has too many blocks that might increase complexity. Not sure if just three people could handle it for the Chipathon time frame.
- For external signals, it is better targeting lower frequency as there is a limitation with analog pads, unless you plan to develop your own RF IOs, that could add an extra chall

### Approval reason
- Fewer than 3 reviews were submitted.
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A02`

**Status:** ⚠️ Not enough reviews

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- Experience with IHP open pdk tapeout > Good
- Good overall plan of the design.
- Need clarity on few things before making sure it is a feasible design for Chipathon:
- Anyway you can show the complexity eg. lines of code, verification time, chip area
- More detail is required on the interface like how are reading/writing weights and calculated valu

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A03`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.17 column H avg; min 2; max 2.5**
- Feasibility: **2.33 column H avg; min 2; max 3**

### Reviewer remarks
- Good architectural plan but looks ambitious unless you provide some implementation plans:
- Architecture of each block: ADC, DLL, gain and offset correction and estimate time.
- Suggestion: trim the plan to 50 M/S ADC with gain/offset correction.
- Timing skew calibration is not needed at this performance level (convice yourselves with a calculation)
- A full array requires 128 caps, not 256. The advantage of using split caps is questinable at the 8 bit level
- Is digital gain/offset correction on chip?
- This is an interesting proposal for interleaved DAC architecture.
- I fill is missing some details on the ADC architecture itself, and how you plan to do the corrections, is it via trimming? is it done in the analog or the digital side? I would suggest in analog.
- Also, it is missing some specs for the ADC like the voltage and the target ENOB, SIN

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A04`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **2.25 column H avg; min 2; max 2.5**
- Feasibility: **4.00 column H avg; min 4; max 4**

### Reviewer remarks
- Manageable specifications.
- Next is to come up with a circuit architecture of the block details.
- Suggestion: Stick to folded cascode to keep the scope manageable
- It is a good project in the analog domain and useful for many applications.
- The specs are achievable for the current node.
- I think you can have some flexibility on the current consumption, although all we want to have lower power consumption, I think guaranting specs like stability and PSRR may have higher priority.
- Be careful with the compen

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A05`

**Status:** ❌ Not approved

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **1.25 column H avg; min 1; max 1.5**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- Good project with an overall plan but more detail needed:
- Come up with realistic spec for the LDO and BGR
- Stick to simple architectures: -For BGR, a simple self-biased (opamp-less) architecture will give good temp stability without complexity.
- For LDO stick to a telescopic, if you can manage, else a folded cascode to avoid frequency comp comp
- The project is an interesting analog block that can be used in several applications.
- In the specs is missing to the define your dropout, as it will determine the pass transistor size, and also the load capacitance, that will influence in your stability margin and PSRR.
- When talking about a dual ratio, I was expecting two outputs but from diagra

### Approval reason
- Fewer than 3 reviews were submitted.
- At least one Documentation score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A06`

**Status:** ⚠️ Not enough reviews

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **2.00 column H avg; min 2; max 2**

### Reviewer remarks
- Although all digital, a good IP for the open-source community
- It has enough complexity for this chipathon except that it is all digital so make a case for silicon proof.
- If you plan to put the feedback loop out side the chip and speed is not an issue, do it through a serial bus like SPI.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A07`

**Status:** ⚠️ Not enough reviews

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **2.00 column H avg; min 2; max 2**

### Reviewer remarks
- Good project and plan for this chipathon.
- Next step should be to work out the architecture details, design and verification plan so the committee can estimate the feasibility of the project

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A08`

**Status:** ⚠️ Not enough reviews

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **2.00 column H avg; min 2; max 2**

### Reviewer remarks
- Very good project with a manageable spec except maybe for Phase noise.
- Main challenge is the modeling of RF circuits in GF180MCU since RF models either don't exist or are limited.
- Inductors take a up a lot of space so that is the something you have to model and layout as quickly to give the team an idea on how much space will be occupied.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A09`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **4.00 column H avg; min 4; max 4**

### Reviewer remarks
- Very good project choice for Chipathon! QSPI controller are useful for many microncontroller application with limited or no onchip flash/RAM.
- It will probably be helpful for some projects in this Chipathon interfacing external flash
- Good plan and documentation.
- An interesting project for serial communication development.
- I would suggest checking if the available IOs, might be useful for the target frequency and voltages. Otherwise might need to think in developing custom IOs (that would take more time of verification).
- Interesting approach for debugging using UART.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A10`

**Status:** ⚠️ Not enough reviews

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- Very good project for this Chipathon.
- Good overall presentation of the plan
- Next: figure out the complexity for design and verification to convince the team that it is a feasible project.
- FYI: There is typo in the area estimate

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A11`

**Status:** ⚠️ Not enough reviews

**Review count:** 0 (minimum required: 3)

### Average scores
- Documentation: **0.00 avg from column H; no individual scores found**
- Feasibility: **0.00 avg from column H; no individual scores found**

### Reviewer remarks
- No reviewer remarks were extracted from the row-2 review comments.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A12`

**Status:** ⚠️ Not enough reviews

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- Very good project for this platform esp. the reproducible goal.
- Two things you want to get an idea quickly to convince the comittee:
- Detail implementation plan to show the project is whitin the scope
- an estimate of an area of the design

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A13`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.67 column H avg; min 3; max 4**

### Reviewer remarks
- Vanilla low-speed SAR ADC
- Realistic scope definition
- Well-defined execution and verification plan
- 8-bit SAR-ADC is a very good open-source IP when silicon verified.
- Binary wieghted DAC should be good enough for 8-bit
- 200 run monte carlo is good enough as long you see normal distro
- Going from 15mV to 2mV offset will require you increasing the area by (15/2)^2 roughly 50X assuming your Vt dominated by the input pair. That's brute force. You
- Classical topology for the SAR ADC.
- Comparator offset requirements depends on your reference and resolution. In your proposal that point is not clear.
- Also, not clear the target sampling frequency. This might affect the sizes for your capacitors.
- It is good that you have simulated the comparator. However, seems to have a systematic offset aro

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A14`

**Status:** ❌ Not approved

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **1.00 column H avg; min 1; max 1**
- Feasibility: **1.00 column H avg; min 1; max 1**

### Reviewer remarks
- Good project proposal for this chipathon
- It is not clear if the proposal is for the kangaroo12 hash function or the entire system.
- The questions are related to the feasability of the implementation of the hash function but that is something the committee may not be able to provide
- My suggestion is to focus only on the kangaroo12 and come up w

### Approval reason
- Fewer than 3 reviews were submitted.
- At least one Documentation score was 0 or 1.
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A15`

**Status:** ❌ Not approved

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **1.00 column H avg; min 1; max 1**

### Reviewer remarks
- Good and appropriate project for the track but need more documentation including
- Are you designing the SRAM as well ?
- Are the multipliers custom build or synthesized ?
- This seems area intensive so quick estimate on the area will give the committee an idea on the feasibility.
- PIN/PAD interfaces.
- What is the interface protocol and is it pa

### Approval reason
- Fewer than 3 reviews were submitted.
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A16`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **2.25 column H avg; min 2; max 2.5**
- Feasibility: **2.50 column H avg; min 2; max 3**

### Reviewer remarks
- Foundational blocks (BGR/SPI/etc) are good addition for this track.
- For cryogenic test: remeber the models are only valid from -40C to 125C. So please address how you are going to test with that limitation.
- Plan for one IP (eg. BGR) and add the rest as time permits.
- Create a design and verification plan for reproducibility.
- Interesting project with several building blocks that can be resuable for next projects.
- Dealing with on-chip sensor might be difficult as PDK devices where not modeled for ultra-low temperatures. You need to find a way how to overcome this challenge. Also, might require some strategies as trimming adjustment for the value after it is manufacture

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A17`

**Status:** ❌ Not approved

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **1.50 column H avg; min 1; max 2**
- Feasibility: **2.50 column H avg; min 2; max 3**

### Reviewer remarks
- A good suitable project for this track
- Detail documentation and clarifications required including
- The block diagram is a generic filter architecture without details involving your architecture for eg.
- How are you tuning the center or cutoff frequency.
- How are you converting from a low-pass to band-pass filter
- How did you come up with the
- The proposal is interesting as a reusable analog block.
- How do you plan to do the programmable side of your proposal. What do you plan to tune, resistors, capacitors. Are they going to be on-chip, off chip?
- For the OTA work as integrator is good to have 1 or 2 decades UGB in open loop higher than the maximum target frequency.
- Some specs are m

### Approval reason
- Fewer than 3 reviews were submitted.
- At least one Documentation score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A18`

**Status:** ⚠️ Not enough reviews

**Review count:** 0 (minimum required: 3)

### Average scores
- Documentation: **0.00 avg from column H; no individual scores found**
- Feasibility: **0.00 avg from column H; no individual scores found**

### Reviewer remarks
- No reviewer remarks were extracted from the row-2 review comments.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A19`

**Status:** ❌ Not approved

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **2.00 column H avg; min 1; max 3**

### Reviewer remarks
- Purely digital
- Proposal lacks specifics, such as workload target
- How was it determined that the design fits without fixing array size, etc.?
- Ambitious project, given all the required pieces, (SPI, etc.)
- Although the project fits the track well, it lacks some crucial details:
- Is the SRAM part of this project's scope ? There are no SRAM IPs for this project that I know of. So this is a critical assumption.
- The interface details are lacking
- the size 2.9mm X 2.9mm is the entire die! I don't think the project can take the entire die space and how

### Approval reason
- Fewer than 3 reviews were submitted.
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A20`

**Status:** ⚠️ Not enough reviews

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- A digital-only FIR filter is fine but provide more documentation including
- The range of frequencies you are targeting
- Provide detail analysis on how designers can calculate coeeficients to customize the filter
- Also provide details for designers to reporduce this on different technologies.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A21`

**Status:** ❌ Not approved

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **1.00 column H avg; min 1; max 1**
- Feasibility: **1.00 column H avg; min 1; max 1**

### Reviewer remarks
- It is a good idea to create an open-source ADPLL IP for application that tolerate higher phase noise or jitter.
- Based on your block diagram, you are planning a 1 GHz DCO which maybe challenging for this technology so elaborate on the DCO architecture.
- An all-digital PLL has the advantage of reproducibility but document clearly the portions you

### Approval reason
- Fewer than 3 reviews were submitted.
- At least one Documentation score was 0 or 1.
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A22`

**Status:** ❌ Not approved

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **1.50 column H avg; min 1; max 2**
- Feasibility: **2.50 column H avg; min 2; max 3**

### Reviewer remarks
- Although it is a good IP to have in the open-source community, this IP does not necessary require a silicon proof. A FPGA implementation should be credible enough since the frequencies invloved are very low.
- Having said that, a detail architecture with case why a silicon proof will be helpful or hardened IP in GF180 will be useful.
- The proposal is interesting in terms of having a flexible serial communication module.
- Keep in mind that all the serial communication blocks needs to handle external signals, so you need to check if avaialble IOs are compatible with the specs required by the protocols. Likely is the case, but in case not, it will move to the field of IO developme

### Approval reason
- Fewer than 3 reviews were submitted.
- At least one Documentation score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A23`

**Status:** ❌ Not approved

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **1.33 column H avg; min 1; max 2**
- Feasibility: **2.67 column H avg; min 2; max 3**

### Reviewer remarks
- Based on existing 65nm design
- Not much documentation provided
- Design seems to require high common mode rejection for the comparator. How is this achieved?
- Only 2 designers, but this could be realisic, given that there is an exisitng design
- Key design innovations should be highlighted for eg. how the resistor biasing only in the 2 LSB capacitors is reducing the entire cap by 8X
- The output shows as 8-bit, is it a typo ?

### Approval reason
- Fewer than 3 reviews were submitted.
- At least one Documentation score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A24`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **2.67 column H avg; min 2; max 3**

### Reviewer remarks
- Inverter-based delta-sigma modulator
- I would not use ring-amps to keep this project manageable
- Specs are missing
- To keep the project manageable I would shoot for a 1st-order to keep stability issues out of the picture.
- If reducing ring-amp to an inverter is possible then that will add to feasibility.
- And then you can add proper documentation and automation to make it a reproducible desig

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A25`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.17 column H avg; min 2; max 2.5**
- Feasibility: **2.67 column H avg; min 2; max 3**

### Reviewer remarks
- Basic 10b SAR
- Not much documentation provided
- Split array may not be needed at 10b level, for simplicity
- Specs are reasonable, FoM is ambitious
- Feasible specs for 10-b SAR ADC
- Add more detail to documentation
- Plain binary instead of split DAC will simplify design and layout and save time.
- Add a plan for making it a reproducible design for the open-source community
- It is good starting with behavioral, but keep in migh that at the end you need to implement it with real devices, so better face the non-idealities from the begining.
- Also, if you feel struggle with the digital side implementation, you can always use digital cells and implement the logic usign them.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A26`

**Status:** ❌ Not approved

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **1.00 column H avg; min 1; max 1**
- Feasibility: **2.00 column H avg; min 2; max 2**

### Reviewer remarks
- A stand-alone branch predictor with a serial interface through the PAD interface may not add much value for silicon proof IP.
- Instead, having the whole core implemented in FPGA and testing at-speed will add more value.
- 100 MHz communication through the PADS will require meticuluous detail design to make it work.

### Approval reason
- Fewer than 3 reviews were submitted.
- At least one Documentation score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A27`

**Status:** ⚠️ Not enough reviews

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **2.00 column H avg; min 2; max 2**

### Reviewer remarks
- If implemented, will be a good addition to open-source IP
- Will need more detail documentation of the proejct
- To answer some of your query's:
- 50k gate design should not be an area issue.
- Not sure about frequency locking attacks
- Top metal can be used to shield from EM attacks.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A28`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- Good and feasible project for Chipathon
- Next step is to add more detail in the documentation
- Show the circuit architecture
- Devices types to be used
- PIN list & output currents
- Verification methodology for reproducibility
- Interesting project as foundational block.
- The specs are described qualitative but we might need numerical values.
- Some that are missing is the power supply, the PSRR, the temperature coeficient, etc.
- Missing the architecture you plan to implement. Conceptually is ok, but is missing how you plan to implement the corrections.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A29`

**Status:** ❌ Not approved

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **1.67 column H avg; min 1; max 2**
- Feasibility: **3.17 column H avg; min 3; max 3.5**

### Reviewer remarks
- Proposal lacks details
- Scope looks OK
- Not sure why opamp is part of design
- Keeping the resoultion low and architecture simple, this is an appropriate project for this track.
- Now we need more detail documentation
- Show the circuit architecture
- PIN list
- Design and verification methodology for reproducibility
- It is an interesting block to be reused in different other projects.
- I understand that the output is voltage and not current. Based on that, you need to adapt the topology to make it work. Considering that the voltages in internal nodes should be higher than ground, so you may need to use a reference voltage as common mode voltage.
- Need to defi

### Approval reason
- At least one Documentation score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A30`

**Status:** ⚠️ Not enough reviews

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- a tiny RISCV is a good project for this track.
- Now we need more detail documentation
- A detail block diagram showing the interfaces clearly:
- The external PIN/PAD required.
- Internal connections to other track-A IPs eg. ADC, DAC and possibly the QSPI from A9
- External Flash
- Design and verification methodology for reproducibility

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A31`

**Status:** ❌ Not approved

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **1.67 column H avg; min 1; max 2**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- Basic 8b SAR
- Not much documentation provided
- Keeping the resolution to 8 bits and the architecture to SAR makes it a feasible project.
- Now we need more detail documentation including
- Detail architecture of the SAR ADC
- Device types to be used.
- PIN list and any internal interfaces.
- Design and verification methods for reproducibility.
- It is a feasible project.
- Maybe is missing the target sampling frequency.
- Also it is good to have some targets for the INL, DNL, ENOB, SINAD, FoM. You can use as reference other designs for the same topology.

### Approval reason
- At least one Documentation score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A32`

**Status:** ⚠️ Not enough reviews

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **2.50 column H avg; min 2.5; max 2.5**

### Reviewer remarks
- Interesting project for a PLL
- Be aware that maybe the digital side might require the use of some custom cells instead of the standard ones.
- There is missing specs for the PLL (range of frequencies, power supply, etc).
- Are you planning to design the LDO/bias generator?
- Suggestion: although using AI to generate images could be convenient, it

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A33`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **2.50 column H avg; min 2; max 3**

### Reviewer remarks
- Can't find design info in repo
- Self calibrating SAR
- Using metastability to detect mismatch is interesting, but I don't undertand how it works from the presentation
- What are the preformance specifications?
- The proposed project is 8bit SAR ADC with self-callibration
- The idea for self-calibration is interesting, but maybe we could see it better from simulation.
- What is the use for flag memory?
- There are some missing specs like the voltage supply, the target linearity, the sampling frequency.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A34`

**Status:** ⚠️ Not enough reviews

**Review count:** 0 (minimum required: 3)

### Average scores
- Documentation: **0.00 avg from column H; no individual scores found**
- Feasibility: **0.00 avg from column H; no individual scores found**

### Reviewer remarks
- No reviewer remarks were extracted from the row-2 review comments.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A35`

**Status:** ⚠️ Not enough reviews

**Review count:** 0 (minimum required: 3)

### Average scores
- Documentation: **0.00 avg from column H; no individual scores found**
- Feasibility: **0.00 avg from column H; no individual scores found**

### Reviewer remarks
- No reviewer remarks were extracted from the row-2 review comments.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A36`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **2.38 column H avg; min 2; max 3**

### Reviewer remarks
- This is a good project and has some great ideas. I like this project. I am a little concerned with the complexity of the SPI interface with the SAR ADC
- it is important you try to get your ADC working first and then approach the SPI; however, it will be good to do this as fast as possible (at least on a first pass). You can can always re-spin thin
- The proposed projects is an ADC with SPI communication. The idea is interesting, however, you should dose your efforts between the ADC and SPI blocks. Maybe is not a good idea understimate the design of the ADC, while conceptully might be straightforward, reaching decent specs might not. Need to define the architecture you will use. The tipe of inp
- A useful block proposal and the high level goal is clear. However the ADC side (which will be the core technical challenge) is underspecified. The project is feasible if the ADC target is kept realistic and the team carefully balances effort between the ADC and the digital interface
- I cannot clearly understand how unique of the high-level proposal.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A37`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **2.00 column H avg; min 2; max 2**

### Reviewer remarks
- he ideas has some scientific merit; however, I am a little concerned with the complexity of the project. I do not see much information other than registers and a SPI interface. You indicate memory in your design but this may be difficult with the complexity of the other units. I would suggest abandoning that portion unless you want to do something
- The proposal has a very meaningful idea and the github repo shows some real early work. However, the scope seems too large for GF180 and the Chipathon timeline. I would strongly recommend defining a much smaller minimum tapeout target and a more ambitious "stretch goal"
- Moreover, integrating a 16 KB instruction memory (IMEM) and an 8 KB data memory (DMEM) on GF180 would be quite challenging, and I would like to see more discussion on the integration.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A38`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **2.50 column H avg; min 2; max 3**
- Feasibility: **3.13 column H avg; min 3; max 3.5**

### Reviewer remarks
- This is a great idea and I like this project despite it being somewhat challenging. It might be good to focus more on the LNA than anything else
- I/O cells are notoriously difficult to test completely (mainly due to resources and testing procedures). You can also come back to putting the ESD cell and experimenting with the reactance. As mentioned
- I know you are working in the development of RF IOs that I consider a great initiative. However, I would recommend defining the target specs for all your blocks and dose the efforts. As you are designing an LNA, you might need to target a specific noise level for the circuit. How do you plan to implement the adjustable bias? will it use a digital w
- This is a strong proposal. The technical direction is valuable and novel for GF180. Would benefit from clearer specs for both LNA and ESD assumptions. Also, since testing is a big component for this year, testing plan for ESD should be discussed.
- I am personally very interested in this kind of fundamental device development. However, the proposal should define clear objectives, evaluation criteria, and target performance metrics. This would make it easier to assess both the technical feasibility and the expected impact of the proposed work.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A39`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **2.25 column H avg; min 2; max 2.5**
- Feasibility: **2.88 column H avg; min 2; max 3.5**

### Reviewer remarks
- This is a super project
- like the complexity of it but also its something manageable. Simulation is super critical to this design; however, also your flow be important. Would like to see some more information on the error amplifier as well as other schematics. Work on trying to ramp up the schematic/simulation early in the timeline I am a little c
- LDOs is a great building block required in several PM circuits. Suitable for the current track. In the specs is good to define the range of load capacitances and ESR that will handle. You can use typical values. PSRR is an important spec in LDOs and might be included in the table of specs to target. Also think in the load regulation and line regula
- This is a practical and feasible proposal. It is obviously very useful for mixed-signal systems, but the topology is fairly conventional. so the real value will depend on how well they define and achieve low-noise low-dropout and high-PSRR targets.
- The proposed circuit is a relatively simple series regulator and does not appear to introduce a particularly novel approach. To strengthen the proposal, it should define more specific design targets or unique features that clearly differentiate it from conventional regulator designs.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A40`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **3.67 column H avg; min 3; max 4**
- Feasibility: **3.67 column H avg; min 3.5; max 4**

### Reviewer remarks
- This is an extremely ambitious but good project. I love the breakdown of the groups and their duties. I would suggest frequent meetings to update everyone on their status but keep those meetings brief to maximize impact and progress. The complexity is the limiting factor of your design. As stated before, this project is ambitious and will require l
- A very strong proposal with clear goal and technically interesting. The github repo and docs show strong preparation.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A41`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **2.50 column H avg; min 2; max 3**

### Reviewer remarks
- great idea. But, this project is fraught with complexities that may be overwhelming. I might suggest focusing on the DAC first and see if you can get that working. Frame buffers are not straight forward in this project. Why wishbone? Why not AHB or something. Many open-source processors use these AHB or AXI equivalent bus structures. How do y
- Interesting project to output a VGA peripheral. Although many of the specs might be defined by the protocol, it is would to include them in the documentation, like the clock frequency, the DAC voltage, etc. Regarding the DAC, be careful about the specs for implementation, which topology are your planning to use? also be careful with maximum frequen
- This is a useful and well motivated proposal. However the scope is not clear to me. it is missing the key factors that will determine feasability (target res, frame rate, color depth, DAC topology, memory, and so on and so on)
- The proposal is based on a simple RGB frame buffer and DAC architecture. However, I could not find the detailed specifications, such as the display resolution, frame rate, or memory requirements. Including these specifications would help clarify both the uniqueness of the proposal and its technical challenges.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A42`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **3.25 column H avg; min 3; max 3.5**
- Feasibility: **3.38 column H avg; min 3; max 3.5**

### Reviewer remarks
- excellent proposal with a great timeline. The Razavi reference is a great item for this project
- I would suggest studying that one well. I am not lying in that this project is not easy
- it's challenging from the design and implementation points of view separately. I might suggest relaxing some of the constraints. Your timeline might be good
- The goal of the project is clear and feasible for the time frame of the contest. Good that the specs were included in the presentation as well as the estimations for are and pins. Good that you have included the full proposal. Although there are PDKs that have separated domain for core and IOs (like IHP) in GF we don't have that separation, so you
- An overal strong proposal. It has a very ambitious output range (0.1 to 1.2 GHz) but the documentation and verification plan gives confidence. I would suggest a minimum goal and a "stretch" goal for a more realistic achievable outcome.
- I am pleased to see a PLL proposal, and the time-domain objectives are clearly defined. However, I would also like to see frequency-domain performance targets, such as phase noise, jitter, loop bandwidth, or lock time specifications. Including these specifications would make the design goals and technical challenges much clearer.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A43`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **2.25 column H avg; min 2; max 2.5**
- Feasibility: **2.88 column H avg; min 2.5; max 3**

### Reviewer remarks
- I love the ambitiousness of this project; however, I am not going to lie and this project is not easy. You have lots to be worried about from the analog and digital point of view. You do have a great repo with some good planning involved
- kudos to you on that. As I have said to other groups, making sure your flow works is important. Test this on a
- Interesting project to create an USB audio interface. Please, define the specs for your DAC, frequency of operation, resolution, voltage, etc. Seems that you are not providing power to the output, just audio signal, in any case, need to assess the output characteristics to prepare your DAC. Not sure what topology are you planning for your DAC. The
- An interesting and valuable proposal and the team background gives confidence. However the proposal is missing some key specs information and PHY and logic assumptions. For a more realistic successful outcome, I suggest the audio DAC to be implemented as minimum requirement and the full USB compliance as a stretch goal.
- I like this audio application, and the target as a USB dongle DAC is clear. However, the proposal should include key specifications such as the sampling rate, audio resolution (bit depth), dynamic range, and target SNR. In addition, if the DAC operates from a clock source other than the USB 48 MHz clock, the proposal should explain the data synchro

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A44`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **2.63 column H avg; min 2; max 3**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- great project! Great complexity combined with ideas. I applaud you for good output and targets. I know things are early here but I do not see much detail on ideas other than the block diagram. Suggestion is focus on flow along with simulation early on in the process. You do have the repo forked so that is a good start.
- The goal is to the build a 8bit 2MS/s Good point to have the list of specifications. It follows the clasical topology for the SAR/ADC. Probably the sample and hold block might be part of the CDAC array. As you are planning to work with relatively high frequency for an ADC, it is important a good characterization of the capacitive DAC including the
- A solid proposal with clear and reasonable targets. CDAC post layout monte-carlo seems like will be a must here so the team should consider a plan for this. I would suggest a "minimum" frequency goal and a higher frequency stretch goal.
- Seems good target specifications list, yet there is no clear application target.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A45`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.67 column H avg; min 2; max 3**
- Feasibility: **2.17 column H avg; min 1.5; max 3**

### Reviewer remarks
- very ambitious project. This project is not easy as the RISC-V processors of any element are not simple. I would suggest simplifying some things like reducing the picosoc_mem or even removing. 256 words, which I believe is the default, is just big even for gf180mcu. 8KiB SRAM is almost impossible given the technology, timeline, and other issu
- First of all, seems like project name in this proposal review sheet is outdated. A very ambitious and very useful project proposal. I am concerned about the ambitious goals given the timeline and the background of the team (undergrad students). I am not doubting their ability or drive, but I think the scope should be narrower. The proposal should h
- The proposal appears to be feasible for a simple 32-bit RISC-V implementation. The concept is straightforward and seems achievable within the project’s timeframe.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A46`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.67 column H avg; min 2; max 3**
- Feasibility: **3.00 column H avg; min 2; max 4**

### Reviewer remarks
- Great idea but SRAM is typically not done as a standard-cell. Scan DFF are also notoriously difficult for characterizers, even commercial ones. I would suggest focusing on other cells first and then go from there. How are you going to test this design
- will you synthesize + pnr this with another simple design. I would suggest trying your XNOR/XOR
- Extending the SC library is super useful. My concern is the scope and targets. Especially the SRAM portion needs clearer targets (memory size, R/W margins, operating frequency, power, area, so on and so on.). Also not sure what "radiation tolerant" means in measurable terms. I would recommend narrowing the minimum deliverable to a small, fully char
- I am personally very interested in fundamental device development, such as standard cells and SRAMs. Since this proposal focuses on a radiation-tolerant SRAM architecture, it should define clear target specifications, such as radiation tolerance, memory size, operating frequency, power consumption, and area. Including these performance targets woul

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A47`

**Status:** ❌ Not approved

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.33 column H avg; min 2; max 3**
- Feasibility: **1.67 column H avg; min 1; max 3**

### Reviewer remarks
- This project although nice is just too complex I would suggest if you want to try this, you focus on something smaller
- it's not that you cannot achieve this. It is just that I have done many of these types of ideas and they tend to be complex even for a team of 20 people. I do not see much information other than some words about TinyML and RISC-V
- The proposal is very ambitious but it is too vague for the stated ambition. It is not clear to me whether the team is building a new CPU, extending an existing RISC-V core, implementing a standalone accelerator, adding compiler/toolchain support, or defining a minimal custom-instruction subset. Not sure if this is feasible in GF180 and the Chipatho
- The proposal combines a RISC-V processor with an LLM engine, which is an interesting concept. However, I could not find a detailed block diagram or architecture showing how the LLM functionality is implemented. It would strengthen the proposal to explain the implementation approach, including the role of the LLM engine, the hardware/software partit

### Approval reason
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A48`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.33 column H avg; min 3; max 4**

### Reviewer remarks
- This is a great project
- focus on the fault injection detection module first and then move forward to other things. I like that you have several members on your team
- might be good to assign tasks to them to make this project work more efficiently. Getting flow + simulation working early on the process is key for this project
- focus on that firs
- This is a strong proposal. I have some questions but overall the high-level architecture is understandable. The main missing details are the quantitative detection targets and characterization plan. Feasibility is good for a proof-of-concept digital detector.
- I am not a specialist in TRC applications, so I cannot fully evaluate the technical details. However, the proposal appears to be well structured and seems suitable for demonstrating the intended functionality.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A49`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **2.38 column H avg; min 2; max 3**
- Feasibility: **2.75 column H avg; min 2.5; max 3**

### Reviewer remarks
- This is another good project. I like the Ideas but keep it simple by working on an element of your design first and then incorporate the feedback loops. Great reference in the presentation to work off of
- this reference is a journal with lots of work involved. It might be good to simplify as much as you can to make this thing work well. How do you
- The goal is to generate an asynchronous 8-bit SAR ADC. Although don't have a global clock that controls the timing alongside the circuit, you need to generate internally clock signals that trigers the flow, S&H, the SAR digital module, the CDAC and comparator. Need to be careful when designing these pulses as you need to ensure all other signals in
- This is a reasonable proposal for a very useful low-power mixed-signal building block. The target of sub-150 uW power is interesting, and the architecture is a sensible fit for this target. However, the documentation is sparse and does not define the key success metrics (sampling rate, input range, supply/reference assumptions, ENOB/SNDR/SNR, INL/D
- The proposal targets a low-power 8-bit SAR ADC, which appears to be feasible. However, it does not define key specifications such as the operating frequency, linearity (INL/DNL), ENOB, SNR. Without these target specifications, it is difficult to assess the technical challenges and the novelty of the proposed design.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A50`

**Status:** ❌ Not approved

**Review count:** 0 (minimum required: 3)

### Average scores
- Documentation: **1.00 column H avg; min 1; max 1**
- Feasibility: **1.00 column H avg; min 1; max 1**

### Reviewer remarks
- No reviewer remarks were extracted from the row-2 review comments.

### Approval reason
- Fewer than 3 reviews were submitted.
- At least one Documentation score was 0 or 1.
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A51`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **2.75 column H avg; min 2; max 3**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- I like this project
- its cool and has some great ideas. I am going to be a little motivational and try to work on something novel about your design (e.g., power efficiency, noise). I think the project is great but it would be good to focus more on an objective here (its still a great idea). 3 team members is going to make this more challenging
- Interesting proposal to implement a SAR ADC with sub-2 radix DAC. It is missing to specify the target frequency. As it using redundancy it likely will use more pulses than the conventional, so take into account when defining the clock and sampling frequency. You mentioned single-command reproducible flow, which might imply a kind of automation in s
- This is a strong and thoughtfully prepared proposal. The asynchronous sequencing and sub-radix-2 redundancy are real differentiators from other standard SAR ADCs, and the documents shows good planning. The main weakness is that several key specifications still missing (sampling rate, input/reference range, unit capacitor size, redundancy radix/weig
- The proposal targets a 10-bit SAR ADC, but it does not define the key design specifications. It would be helpful to include target specifications such as the sampling rate, ENOB, INL/DNL, SNR, power consumption, and operating voltage. Without these target values, it is difficult to evaluate the technical challenges and the design objectives.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A52`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **2.25 column H avg; min 2; max 2.5**
- Feasibility: **2.63 column H avg; min 2; max 3**

### Reviewer remarks
- Great presentation and idea is ambitious I like this project but could run into a complexity project. I would suggest trying to work on one block and implement with the flow to see if things work. Then, you can revisit things as you go. A digital decimation filter is possible in digital but might be large in scope
- might want to wait until later i
- This is an interesting proposal for a sigma-delta ADC. The blocks are identified for each of the components in digital and analog domain. The sampling frequency is not matching the units in specs table. As bandwidth spec not sure for which element are you refering (the compartor, the OTA?). Normally, sigma-delta are intended for low frequency input
- This is a useful mixed-signal building-block proposal, but the architecture is fairly conventional. My main concern is specification consistency and feasibility. The documents do not fully agree with eachother. The targets need to be reviewed carefully to make a physically consistent ADC specification. I think the plan overall needs a bit more deta
- The proposal targets a 12-bit Delta-Sigma ADC, which is an interesting design. However, achieving a 2 MHz sampling rate appears to be quite challenging. The proposal would benefit from more discussion of the design approach and the key performance targets, as well as an explanation of how the target sampling rate will be achieved.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A53`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **3.13 column H avg; min 3; max 3.5**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- I love this design
- its great and has great applicable towards our area. I am not understanding why you are using a BIST engine for this design What do you plan on measuring? How do you plan on testing the TRNG? You have a great group of members on this project
- might be advantageous to put specific roles for each member as larger teams tend to g
- The idea of creating a true radom number generator is interesting. The ring oscillator, although can be seen simple might imply several verifications, specially with parasitics, to ensure targets the desired frequency. Also, consider that it will have variations across PVT. Not sure if planning to use pure inverters or starved inverters for the imp
- This is a strong proposal for a very useful, valuable and reusable block. The block diagram is understandable and the pinout is more concrete than many of the other proposals. The key here is I think proving the entropy quality. Feasible as a proof-of-concept, but the “NIST-compliant” claim should be treated carefully until the entropy validation p
- The proposal for a random number generator appears to be feasible on the GF180 platform. However, it does not define the target design criteria, such as randomness quality, statistical performance, or the verification methodology. The proposal would be stronger if it included target metrics and evaluation methods, for example, compliance with stand

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A54`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **2.00 column H avg; min 2; max 2**

### Reviewer remarks
- Your presentation was over the limit in time and slides This project is complex and although a great idea, SRAM implementation is going to be largely time consuming. I would suggest trying to break this down into a smaller element. For designs, I always advocate working bottom up with a design. That is, start simple and then expand as you go. Dont
- The proposal does not include a block diagram, data flow, or input/output information. As a result, it is difficult to understand how the system works and how the proposed functionality would be implemented. Including a clear architecture diagram and signal flow would make the proposal much easier to evaluate.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A55`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.17 column H avg; min 2; max 2.5**
- Feasibility: **2.50 column H avg; min 2.5; max 2.5**

### Reviewer remarks
- Nice program but not a lot of detail. Good team effort but might be easier to give specific tasks to everyone instead of "digital" or "analog". Will give people purpose and make coordination easier Look at the PLL reference for Razavi to help
- he's got several great texts and papers In the design sections, there's lots there and might be good to t
- The general idea is interesting. However, it is missing a block diagram that shows the interaction between components. It is good to have selectable outputs however it is missing how many outputs (control input resolution) and in which range. There is not much details on the 16bit sigma delta modulator. Including an SPI block also will require an e
- The proposal includes an LDO, bandgap reference (BGR), and fractional-N PLL, which is an interesting combination. However, it does not include a block diagram or detailed target specifications. Without a clear system architecture and performance targets, it is difficult to evaluate the technical challenges, feasibility, and overall design objective

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A56`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- Wow this is a big project and may be something that is hard to complete for a 2-person team. SRAM is notoriously difficult and having a 256x8 may be difficult. Would suggest working from the bottom up in terms of complexity. That is, get something working and then expand if successful. Time is your enemy with this project. You do not have a lot on
- The proposal appears interesting and may be feasible to implement on GF180. However, the presentation would be much stronger if it included a more detailed block diagram and data flow.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A57`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.17 column H avg; min 2; max 2.5**
- Feasibility: **2.50 column H avg; min 2; max 3**

### Reviewer remarks
- do not see much in terms of your initial proposal
- you should work towards expanding this. As indicated previously, your work will be a "living document" (i.e., it will be expanding each day/week). So, keep updating things on this repo. You have a good group but not a lot of definition in terms of what each person is working on. Suggestion is to m
- The proposal is interesting in terms of the multi-channel feature of the SAR ADC. Consider that we don't have 1.8V devices, but 3.3V. So you need to assess of using a low voltage is better alternative for your design. SPI module will also require an extra effort that you need to account unless you have an IP ready to use. For the capacitive DAC nee
- The proposal targets an 8-bit SAR ADC with 8 input channels, which appears feasible. However, it does not clearly explain how each channel is configured or how the overall chip architecture is organized.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A58`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.25 column H avg; min 3; max 3.5**

### Reviewer remarks
- Nice proposal and information UARTs are not that easy to implement and you may have some issues here without prior experience. Check out my text on RISC-V System on Chip book from Elsevier
- there is discussion on UARTs along with some HDL at the website. How are you implementing the SRAM? The schematic review slide link seems empty?? You may want
- The proposal targets a 3x3 convolution accelerator, and it appears feasible to integrate on GF180. The concept is clear and practical. It would be helpful to include more details on the target performance, data flow, memory interface.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A59`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- Interesting project and a good project complexity for the chipathon Might want to define the objective more to give some detail of what you are accomplishing (e.g., simplicity, accuracy). I did not see much in the proposal or repo about further details. You might want to work on defining this more to really give an idea what you are accomplishing T
- The proposal targets a Softmax accelerator, and the objective is clear. However, it does not include a detailed block diagram showing how the accelerator would be implemented. The proposal would be stronger if it explained the internal architecture, data flow, memory interface, and approximation method for the exponential and division operations.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A60`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.50 column H avg; min 3; max 4**

### Reviewer remarks
- This is a fantastic project and great idea. However, I am not going to lie that its easy
- its actually quite challenging especially as you got to 64x8 and higher. However, I think it's a do-able project. Don't see really defined roles for the team members
- will help if you give specific tasks for each member and make each week smoother. Like the
- The proposal targets a small 16x8 SRAM or register-file structure that can scale to 32x8 or 64x8. It would be helpful to compare this approach with a standard-cell-based implementation.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A61`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **2.50 column H avg; min 2; max 3**
- Feasibility: **2.50 column H avg; min 2; max 3**

### Reviewer remarks
- This is a nice project and has some good design objectives. The proposal slides are somewhat vague which could use some clarification and expansion. Much of the details as you go with be a "living document"
- i.e., expanded constantly each day/week; therefore, updating things often is a good idea. I like the project, but not sure of the WL control
- I could not clearly understand how the proposed design operates. A block diagram and a simple explanation of the system architecture and signal flow would make the proposal much easier to follow and evaluate.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A62`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.17 column H avg; min 2; max 2.5**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- Like the proposal. Good references and alluding to the idea in the paper. Well done! Focus heavily on simulation here
- do you have any schematics? Your schematic/layout review slides are empty. Please try to make sure team members have clearly defined roles
- will help you get to the finish line. More detail on interfacing would also be good in th
- The intended circuit is clear in related to circuits that emulates neural synapses. What is not clear is how many of those cells are going to be implemented. Is the intention to build a network with them? Maybe is good thinking on them as pcells that will be used in an application. Otherwise it might be too small for the area available and do not s
- The maximum voltage allowance of the proposed circuit is not clearly described. It is also unclear how this circuit would be implemented on the GF180 platform, including device selection, voltage domain, and reliability considerations.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A63`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.17 column H avg; min 2; max 2.5**
- Feasibility: **2.67 column H avg; min 2; max 3**

### Reviewer remarks
- Wow, this proposal is not easy
- I would highly recommend simplifying things. It's too complex. The idea is a good one but it may not be possible giving the timeline Schematic/Layout review slides are empty Try getting some more team members and honestly focus on the roles more in detail. Giving specific roles to each member will help each member w
- The project aims the development of I3C interface. This is in the scope of IO design. You need to be careful on the IOs that will be used and if the available ones meet the requirements for the protocol. Normally, it requires custom IOs, but better confirm if the available ones are compatible. Think in the voltage levels that supports the protocol
- The proposal targets an I3C interface, which is an interesting and useful function. However, it is not clear how the interface would be verified, or how it would connect to the digital logic side through input and output signals.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A64`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **3.17 column H avg; min 3; max 3.5**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- Great project and have a good objective Schematic hard to read
- might be advantageous to break the xschem schematic up into multiple views Clear objective and good to focus on simulation here
- work out the simulation so you have that working in the beginning Give more defined roles to each team member to make things more collaborative. It will he
- The goal is an interesting analog circuit that takes the difference from two inputs. In specs is missing the voltage of operation. Also, as you planning a fully differential topology yo need a VCM input. Not sure if will be generated or will be provided externally. In any of the cases, is good to expose it to the output, as reference for next block
- The proposal and target application are very clear, and the circuit schematic helps make the implementation easy to understand. However, the proposal does not include simulation results.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A65`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.17 column H avg; min 2; max 2.5**
- Feasibility: **2.50 column H avg; min 2; max 3**

### Reviewer remarks
- This is a good project but find references from Razavi with his texts and papers PLLs are not easy and need lots of simulation and analysis.- focus heavily on simulation and making sure you make sure things work individually and then when connected. If you simulate separately first and make sure you get things achieved, it will help You have a low
- Interesting project to desing a configurable clock synthesizer based on PLL. In the specifications is missing the range of frequencies and the voltage of operation.
- The proposal targets an Integer-N PLL, but the architecture appears to be a simple and generic PLL structure. To evaluate the technical value more clearly, the proposal should include target specifications and response parameters, such as output frequency range, phase noise, jitter, lock time, loop bandwidth, and power consumption.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A66`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **3.67 column H avg; min 3.5; max 4**
- Feasibility: **3.33 column H avg; min 3; max 4**

### Reviewer remarks
- Nice project with some simulation already
- nice Not sure where you got your specifications
- would concentrate on getting things working first Check also references by Razavi in his books/papers Give more detailed roles for each member to help get objectives done each week. The pulses on the modeling seem a little short and not realistic
- Great to see that you have already a model with simulations that shows it working, Good point also the table of specs. The wide operation frequency is an interesting feature.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A67`

**Status:** ❌ Not approved

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **1.50 column H avg; min 1; max 2**
- Feasibility: **1.50 column H avg; min 1; max 2**

### Reviewer remarks
- I am not quite sure what this project is and what circuit you are implementing
- consider detailing this for the project This proposal could use a huge boost in detail
- references too The block diagram of the project is confusing
- is this digital or mixed signal? Consider simplifying the ideas to meet a simplified objective and then work up in co

### Approval reason
- Fewer than 3 reviews were submitted.
- At least one Documentation score was 0 or 1.
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A68`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- This is a nice idea but there's lots here. Might be good to simplify things and work upwards SPI controller information is somwhat weak in what is being provided Make sure you focus early in the process on the design flow for this project
- it will save you a ton of time later in the design if you focus right at the beginning. aes128 can be a bit b
- The proposal appears feasible and suitable as a proof-of-concept demonstration. However, I could not clearly understand the advantages of this approach compared with an FPGA-based implementation.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A69`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.17 column H avg; min 2; max 2.5**
- Feasibility: **2.67 column H avg; min 2.5; max 3**

### Reviewer remarks
- Proposal is not very specific although schematic above in the repo is helpful. Consider giving more details in the schematic review slides Simulation is key on this project
- focus early on getting simulation something you can run easily and often. You could use another team member to help you Also consider giving defined roles for each team member
- This is an interesting analog project that might have several uses for different applications. The target accuracy seems to be challenging, so there will be several tests will need to be done the target is achieved (including MC and post ayout simulation). Trimming will help to achieve the target accuracy. Typically the bangap output is 1.2V. What
- The proposal targets a bandgap reference (BGR), but it is not clear why the output voltage is set to 1.8 V.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `A70`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- Nice name of team :) Nice idea but not a lot of detail in the presentation other than a block diagram Consider specifically giving goals for each team member early in on the project so objectives are easy to complete each week. Making sure you have a good methodology and/or flow for simulating is key for this project. More details on where specific
- Good that already defined the list of specifications. Regarding the supply voltage, consider we don't have 1.8V devices, just 3.3V. So, could be would to assess the best power supply for them. Regarding the reference voltage you need to assess if will be integrated or off-chip. For 1-bit bitstream output, are you refering to the analog side? are yo
- The proposal clearly presents the key design targets, which makes it easy to understand the design objectives. However, the proposal specifies a 1.8 V supply, while the GF180 platform primarily supports 3.3 V devices.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B01`

**Status:** ✅ Approved with comments

**Review count:** 5 (minimum required: 3)

### Average scores
- Documentation: **2.75 column H avg; min 2; max 3**
- Feasibility: **3.50 column H avg; min 2; max 4**

### Reviewer remarks
- Good initail idea.Feasible in the timeframe. Programable gain amplifier. No defined area /inputs or outputs
- Application is clear. Feasible in timeframe. Specifications provided. Define input and output.
- BW and DR enough to detect PM2.5 ?
- Suitable size of target to design in Chipathon schedule. More investigation on I/O will be needed. The input signal may be very small, so analog I/O cell might be a problem. Also, output buffer and I/O cell should be considered for high fidelity output signal to MCU.
- Simple and feasible idea. Not very differentiated, but interesting/relevant

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B02`

**Status:** ✅ Approved with comments

**Review count:** 5 (minimum required: 3)

### Average scores
- Documentation: **2.25 column H avg; min 2; max 3**
- Feasibility: **2.75 column H avg; min 2; max 3**

### Reviewer remarks
- Prototype at circuit level. No trarget application, but a general purpose block. It is doable
- Feasible but need better definition. Block level design, specifications, layout estimation missing.
- PLL design is a challenging issue. I think the feasibility is an issue.
- Highly reusable general purpose circuit. The target contains several blocks and design difficulty looks high, but design is already in progress. The team has many members, so it looks possible to complete design in Chipathon.
- Idea not very clear, but a proptotype is available and it would allow exploring different paths. Needs better definition.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B03`

**Status:** ❌ Not approved

**Review count:** 5 (minimum required: 3)

### Average scores
- Documentation: **2.75 column H avg; min 2; max 3**
- Feasibility: **1.25 column H avg; min 1; max 2**

### Reviewer remarks
- Voltametric sensing. A complex block diagram. Concern about blocks like SPI. Great application. Ambitious.
- Strong application. Ambitious and complex. Involves many blocks and domains. Missing specs and targets.
- This is ambitious project. Compared to the numbers of the teem members.
- The application is interesting and the architecture is clear. The difficulty of design looks very high. The number of blocks is large and the target spec is high, i.e. 12-bit ADC/DAC. To complete design in Chipathon schedule, it looks better to shrink the target or reuse/share some blocks like SPI, clock gen.
- Very interesting, but design is too complex for the timeframe

### Approval reason
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B04`

**Status:** ❌ Not approved

**Review count:** 5 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **1.75 column H avg; min 1; max 2**

### Reviewer remarks
- Microphone input. I2C interface. Would you be using open excisting blocks?
- Application unclear. Missing specs and targets. Might be complex considering mixed signal implementation with multiple blocks
- I am afraid if thie block fits with 1mm squares.
- Interesting target. The target blocks and their specifications are not clear. If includhing whole digital blocks, many other blocks like I2C, clock gen etc. are required.
- Specs/implementation is vague. Design is probably too complex, but some blocks could probably be reused from opensource libs

### Approval reason
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B05`

**Status:** ❌ Not approved

**Review count:** 5 (minimum required: 3)

### Average scores
- Documentation: **2.75 column H avg; min 2; max 4**
- Feasibility: **2.25 column H avg; min 1; max 3**

### Reviewer remarks
- We might need aditional information about the output of the DVL.ADC (can we use excisting block?) . I2C block. Doable but with external blocks
- Novel application. Specs reasonably given. Manageable within chipathon timeframe.
- This is an interesting project. The content look reasonable to me.
- Interesting application. The design of digital blocks looks tough in Chipathon schedule. It looks better to consider to shrink the target to complete in Chipathon.
- Interesting and well defined. Might be too ambitious for the timeframe

### Approval reason
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B06`

**Status:** ❌ Not approved

**Review count:** 5 (minimum required: 3)

### Average scores
- Documentation: **2.75 column H avg; min 2; max 3**
- Feasibility: **1.00 column H avg; min 1; max 1**

### Reviewer remarks
- We need more information regarding the blocks the your team will be fabricating. You should define one specific sensor. The scope is too broad.
- Novel but looks ambitious. Can plan with 1 or 2 in place of 4 sensor reading to reduce scope. Block B not clear. Verify on chip sram support in gf180.
- The project seems to be very challenging. Better to narrow down the project scope.
- Interesting application. But the target archtecture includes so many blocks, so it looks tough to complete all design in Chipathon schedule.
- Interesting, but not well defined and too complex

### Approval reason
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B07`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **3.25 column H avg; min 2; max 4**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- ECG. Instrumentation amplifier, bandpass and filter. Doable in the time frame. Proposed technoilogies
- Feasible. Scope and architecture well defined. Layout area and pin planning done well.
- Interesting application and feasible size of target. Detailed circuit topologies are shown.
- Interesting and well defined. It should be feasible

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B08`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **3.25 column H avg; min 3; max 4**
- Feasibility: **2.75 column H avg; min 2; max 4**

### Reviewer remarks
- ECG. Deterct heart rate variability. Complex topology. They might need to obtain external pre-define blocks like the ADC.
- Novel proposal but ambitious. Suggestion to take some functionality off chip to reduce scope. Top level specs, area planning missing.
- Interesting application. The target archtecture contains many blocks. To complete design in Chipathon schedule, reusing existing design or sharing with other teams are effective on ADC, digital interface, voltage reference and so on.
- Interesting and novel. Might be a bit too ambitious for the timeframe

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B09`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **2.75 column H avg; min 2; max 3**
- Feasibility: **2.50 column H avg; min 2; max 3**

### Reviewer remarks
- Linear Hall Sensor. Good fundamental. He is running alone.
- Nice idea but unsure about Hall sensor implementation and model for GF180. Required to accurately simulate behavior for design. Missing specs and layout info.
- Interesting application. The design looks feasible, but it is better to consider to reuse/share some blocks like bias gen. with other teams. Designing all block by a single-member team might be tough to complete in Chipathon schedule.
- Interesting and should be feasible. Team is a single person

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B10`

**Status:** ❌ Not approved

**Review count:** 5 (minimum required: 3)

### Average scores
- Documentation: **2.75 column H avg; min 2; max 3**
- Feasibility: **2.00 column H avg; min 1; max 3**

### Reviewer remarks
- Bridge sensor. Main component an OTA, SAR ADC. For MEMS sensor.SPI block might be external. Good specifications. Verify the operation frequency.
- Well defined roadmap and approach. Specs given. Feasible design. Suggestion to analyze layout area requirement.
- Only one member can not handle with the system design.
- Interface to MEMS sensors. Good target to design, and the target specs are shown. SPI interface block might be tough to implement in Chipathon schedule.
- Interesting and well defined. Might be a bit too ambitious

### Approval reason
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B11`

**Status:** ❌ Not approved

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **2.25 column H avg; min 1; max 3**

### Reviewer remarks
- Measure voltage and impedance of the battery. Microcontroller might not be inlcuded. Well defined project.
- Industry relevant application. Well defined blocks. Implementation in timframe might be challenge. Suggestion to take some functionality off chip. Layout area estimate should be done.
- 2mV offset calcellation feature using 180nm CMOS is a chllange
- Battery management chip. The target looks doable in Chipathon schedule. Team B13 are targetting similar system, so collaboration with B13 looks interesting.

### Approval reason
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B12`

**Status:** ❌ Not approved

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 1; max 3**
- Feasibility: **2.00 column H avg; min 1; max 4**

### Reviewer remarks
- Creative configuration. We need more information about the Synapse Array to evaluate the feasibility. It will be doable during the time.
- Interesting proposal. Limited system level details, specs, layout considerations
- An interesting proposal, but more detailed information about the archtecture and circuits are needed.
- Simple and should be feasible (provided that synapse circuitry is not too complex)

### Approval reason
- At least one Documentation score was 0 or 1.
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B13`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.50 column H avg; min 2; max 3**
- Feasibility: **3.25 column H avg; min 3; max 4**

### Reviewer remarks
- Monitory battery health. SPI block might be brought from other designs. CAscode and OTA can also be integrated. Doable
- Feasible. Architecture and block planning done with specs. Estimated area and integration might be challenging.
- Battery management IC. Detailed circuits are shown and it looks possible to complete in Chipathon schedule. Collaborating and/or exchanging design with B11 might be interesting.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B14`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.75 column H avg; min 2; max 3**
- Feasibility: **3.25 column H avg; min 3; max 4**

### Reviewer remarks
- Cyclic voltametry. UART and ADC could be obtain from excisting modules.Duable in the timeframe
- Interesting application. Block level planning done. Seems feasible in timeframe. Suggest to plan block and top level specifications.
- Interesting application. Good size of design for Chipathon. You may be able to find UART in existing designs.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B15`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.75 column H avg; min 3; max 4**

### Reviewer remarks
- The circuit is doable in the time frame. Better defifinition of the sensor outputs will be necessary.
- Feasible and practical application. Block and pin level planning done. Suggest to bring out block level specs.
- This project seems to be good and feasible to me.
- Interesting application. It looks good target to complete in Chipathon schedule. Please show more detailed specifications of circuits.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B16`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- Very nobel application. We might need more infomration about the output of the sensors. The propposed circuit seems viable.
- Novel application. Specs and block level planning done. Suggest to plan layout estimate. Seems feasible in timeframe.
- Optimization of SNR of SAR-ADC is a challenge. Because thermal noise is not fully characterized in GF180 PDK.
- Interesting application. The target circuits looks posiible to be completed in Chipathon schedule. SPI module can be shared with other teams or can be taken from existing designs.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B17`

**Status:** ❌ Not approved

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **1.33 column H avg; min 1; max 2**

### Reviewer remarks
- Circuit is doable but this is a 1 person team and the scope is too big. Consider teaming up.
- Application is interseting but need more details about block integration and specs. Several blocks for timeframe look optimistic.
- Only one member cannot perform the system. .
- Interesting application. The target system includes many blocks, so it looks tough to be completed by single-member team. More information (expected impedance of electrodes, working frequency, etc..) is needed.

### Approval reason
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B18`

**Status:** ❌ Not approved

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **2.00 column H avg; min 1; max 4**

### Reviewer remarks
- Very ambicious design. Consider reducing the scope of the project for the short timeframe
- Interesting application. Scope appears ambitious for chipathon timeframe. Consider narrowing it.
- Interesting and high novelty application. The target archtecture is very ambicious, so it looks tough to be completed in Chipathon schedule. It is better to shrink the target.

### Approval reason
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B19`

**Status:** ⚠️ Not enough reviews

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **2.33 column H avg; min 2; max 3**
- Feasibility: **3.33 column H avg; min 2; max 4**

### Reviewer remarks
- Good target for Chipathon. More detailed information of each blocks is needed.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B20`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.67 column H avg; min 2; max 3**
- Feasibility: **2.33 column H avg; min 2; max 3**

### Reviewer remarks
- Consider integrating excisting blocks, specially SPI. The project seems more ambitious than the time allocated for the chipathon.
- Novel application but scope is large. As mentioned in 'Questions' reduce the level of implementation to make it feasible.
- Useful chip is proposed. The proposed archtecture contains so many blocks, so it looks tough to complete all designs in Chipathon schedule.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B21`

**Status:** ⚠️ Not enough reviews

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- Connect to a MEMS sensor. Radiation hardening by design. We need additional iformation about the proposed block diagram. It seems more ambitious than the timeframe for this chipathon. If you have preliminarty designs it will provide additional confidence on the viabiliyt

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B22`

**Status:** ❌ Not approved

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **2.33 column H avg; min 2; max 3**
- Feasibility: **1.00 column H avg; min 1; max 1**

### Reviewer remarks
- Application is interesting. Evaluate whether rad hard models required, might be out of scope. Asses feasibility of implementing proposed blocks within timeframe.
- Clearly defined target. It is interesting, but the target archtecture contains so many blocks to complete in Chipathon schedule. It is better to shrink the target, and/or reusing existing designs.

### Approval reason
- Fewer than 3 reviews were submitted.
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B23`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.67 column H avg; min 3; max 4**

### Reviewer remarks
- It is recommended to use external blocks. Specially the SPI.
- Highle feasible. Can generate good IP blocks for future.
- Good target for chipathon and the design will be highly reusable.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B24`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **2.33 column H avg; min 2; max 3**
- Feasibility: **3.33 column H avg; min 3; max 4**

### Reviewer remarks
- Interesting application and seems feasible. More details to be added.
- Good target for chipathon. More detailed specification of each blocks is needed.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B26`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **3.33 column H avg; min 3; max 4**
- Feasibility: **3.00 column H avg; min 2; max 4**

### Reviewer remarks
- Interesting and novel application. Scope and blocks well defined. Seems feasible in timeframe.
- THe I/O design for IGZO is a design challenge. TEmperature, leakage curent is a dsign issue.
- Good target for chipathon. The details of circuit and target spec are cleary defined.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B27`

**Status:** ❌ Not approved

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **1.00 column H avg; min 1; max 1**
- Feasibility: **1.50 column H avg; min 1; max 2**

### Reviewer remarks
- Application is interesting. Need to add more details and specs in proposal.

### Approval reason
- Fewer than 3 reviews were submitted.
- At least one Documentation score was 0 or 1.
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B28`

**Status:** ⚠️ Not enough reviews

**Review count:** 0 (minimum required: 3)

### Average scores
- Documentation: **0.00 avg from column H; no individual scores found**
- Feasibility: **0.00 avg from column H; no individual scores found**

### Reviewer remarks
- No reviewer remarks were extracted from the row-2 review comments.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B29`

**Status:** ❌ Not approved

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **3.33 column H avg; min 3; max 4**
- Feasibility: **2.00 column H avg; min 1; max 3**

### Reviewer remarks
- Nobel application, concerns about the application of the neurons with the GF fabrication process. This part should be simulated.
- Innovative and well defined application. Scope appears ambitious for timeframe. Consider focusing on architecture that can be realistically implemented and taped-out.
- Interesting application and the target is clearly defined in the presentation.

### Approval reason
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `B30`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.67 column H avg; min 2; max 3**
- Feasibility: **2.00 column H avg; min 2; max 2**

### Reviewer remarks
- Ground penetrating radar. Main concenr ins the Frequency range for this technology. Please verify before proceed. Design might be doable.
- Practical and interesting application. Involved compelx RF architecture and blocks. Implementation in timeframe might be challenge. Add more details.
- Interesting application. Detailed spec, especially the target frequency, is needed. The archtecture is clear, but it contains many blocks. Since it is RF design, so it looks tough to complete in Chipathon schedule.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `C01`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.20 column H avg; min 3; max 4**

### Reviewer remarks
- need to update your block diagrams into proper block diagrams nice to see circuit simulations in the full proposal
- Good to see you have already simulated the blocks. A suggestion in the bias generation for folded cascode, you might consider the wide swing structure to generate the cascode bias One of the objective of open loop simulation is the stability. Some of the loop gain/phase look weird at low frequencies, maybe because the selection of inductance and ca
- The concept appears applicable to the MOSbius platform. However, I could not find sufficient circuit-level design details beyond AI-based estimations, making it difficult to assess technical feasibility and implementation risk.
- Interesting proposal. The block diagram needs to be redone. To improve clarity, please avoid drawing by hand. Do you intend to monitor the internal node signals with test points? Is the 100 pF off-chip load too large?

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `C02`

**Status:** ❌ Not approved

**Review count:** 0 (minimum required: 3)

### Average scores
- Documentation: **1.00 column H avg; min 1; max 1**
- Feasibility: **1.00 column H avg; min 1; max 1**

### Reviewer remarks
- No reviewer remarks were extracted from the row-2 review comments.

### Approval reason
- Fewer than 3 reviews were submitted.
- At least one Documentation score was 0 or 1.
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `C03`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **2.60 column H avg; min 2; max 3**
- Feasibility: **2.20 column H avg; min 2; max 3**

### Reviewer remarks
- check your mixer topologies ... you need quadrature generation!
- The proposed project look a bit ambitious for the time frame we have for chipathon. In block diagram, might be missing what elements will be configured by the switch matrix.
- This is an excellent RF proposal. However, we are concerned that it may be difficult to meet the program timeline, considering the complexity of RF design and the current verification capabilities available to the project.
- This is the first RF proposal that I have seen in the Chipathon. I strongly encourage this new approach to the Chipathon. However, RF work requires more consideration. You need to add test structures (short, open, 50 Ω) for extracting the S parameters and de-embedding pad parasitics. Will you be able to incorporate all this circuitry? Please specif

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `C04`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **3.20 column H avg; min 3; max 4**
- Feasibility: **3.00 column H avg; min 2; max 4**

### Reviewer remarks
- specs are very aggressive focus on one application think in more detail about the application setup and testing and specs
- Good to see some schematic simulations. It could be good to specify what are you planning to do as experiment for this, and what is going to be changed by the bitstream following the MOSbius style. What makes this MOSbius style.
- Generic PLL design proposal, yet it would be interesting how to realize it on MOSbius platform.
- Good proposal. Nice to have already simulations. I agree with LVZ, where is the MOSbius style for this proposal? Please consider also EMI to other group circuits when connecting to MOSbius matrix.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `C05`

**Status:** ✅ Approved with comments

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **2.67 column H avg; min 2; max 3**

### Reviewer remarks
- Need to think more carefully through the use cases of the amplifiers including the component values. Need to think carefully on what measurements to perform and how, i.e. what equipment will be needed + the loading effects ....
- Not clear if going to use on-chip or off-chip capacitors/resistances for the compensation loop. If they were to be off-chip likely will require exposing the pins increasing the required ones. On the other hand on-chip elements will require more area. Need to assess properly which path to follow
- The proposal includes only a high-level block diagram. Detailed circuit architecture and chip area estimates were not provided.
- There are a lot of techniques to be included in the chip. Perhaps two techniques per amplifier would suffice to avoid excessive complexity during integration. I couldn't correctly identify the number of pins you will use. Remember that the dies will be shared with other groups.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `C06`

**Status:** ❌ Not approved

**Review count:** 4 (minimum required: 3)

### Average scores
- Documentation: **1.00 column H avg; min 1; max 1**
- Feasibility: **2.50 column H avg; min 2; max 3**

### Reviewer remarks
- Document the application of the chip and the block diagram better as well as the use cases of the chip; your team is big enough to add the PWM generator on chip if you plan carefully and distribute the work well. I am not sure I understand the title -- make it clearer what you mean or adjust so it better covers the chip function.
- The idea is interesting however, feels incomplete and not grounded. There are missing points on what elements that are going to be configurable and how this fits in the MOSbius style chip.
- I cannot clearly understand how this would be implemented on the MOSbius platform.
- Other teams' PCBs need to include off-chip components. I am not sure if this is a good idea. Will other teams need to buy an SPWM generator? Could you please explain in detail how this can be incorporated into the MOSbius style?

### Approval reason
- At least one Documentation score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `D01`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.17 column H avg; min 2; max 2.5**
- Feasibility: **2.67 column H avg; min 2; max 3**

### Reviewer remarks
- It is not clear in your block diagram where the BGR is going to work. Not clear in your proposal where is the use of AI/LLM, or the automation side. You need to answer why this project is suitable for Track D?
- Pin out and area estimation were presented. Was not clear where "AI/LLMs" are playing a role
- While the target application is clearly defined, the proposal lacks a detailed implementation plan and technical architecture.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `D02`

**Status:** ❌ Not approved

**Review count:** 1 (minimum required: 3)

### Average scores
- Documentation: **0.00 column H avg; min 0; max 0**
- Feasibility: **0.00 column H avg; min 0; max 0**

### Reviewer remarks
- Not presented/shared a video Not much information in github issue

### Approval reason
- Fewer than 3 reviews were submitted.
- At least one Documentation score was 0 or 1.
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `D03`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- Digital blocks, area optimization is the goal. AI code agents embeeded as part of the design flow for verification and debugging. Documentation and intent is clear.
- While the target application is clearly defined, the proposal also suggests the use of AI agentic optimization. However, the actual implementation methodology and circuit architecture are not described in sufficient detail.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `D04`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **2.75 column H avg; min 2.5; max 3**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- Idea is interesting, platform oriented and AI-Native; global open source comunity can test/evaluate/iterate. No proposed circuit, team members looks experience (based on previous years contributions). Focus on Digital flow "Automation", documentation is ok,; however more details peer stage of the flow are needed, it's not clear how the flow is bein
- The AI-assisted design platform and its cloud-based implementation are interesting concepts. However, I could not clearly understand the actual chip design proposal or the technical challenges that the project intends to address.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `D05`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.50 column H avg; min 2; max 3**
- Feasibility: **2.67 column H avg; min 2; max 3**

### Reviewer remarks
- The idea of the gLayout wrapper is interesting however, the abstraction might sacrify the flexibility of gLayout. On the other hand, how this wrapper connects to your goal of RF design? Not clear yet what is your plan for tapeout.
- Wrapper of glayout and align for analog design automation. AI agent+skills will be use as part of the optimization loop, however this loop is just at simulation level; no layout effects are considered as part of the AI optimization strategy. No clear proposal of the circuit to be tapeout.
- It appears that gLayout provides a code-based layout template approach. However, it is not clear how it would be integrated into an AI-driven optimization loop, or how the final target layout would be generated and evaluated.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `D06`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.50 column H avg; min 2; max 3**
- Feasibility: **2.67 column H avg; min 2; max 3**

### Reviewer remarks
- Not sure if audio falls into RF category. Not clear in which stages are going to use AI and in which not. Are you planning to use integrated inductors? Missing to specify what are you planning to tapeout
- use of AI for RF design is interesting, however is not clear in wich stage of the design or in which way AI/LLMs are planned to be use, clarification on this and coumentation will be good for the community to know from a real scenario design intent+ tapeout+meas-results where AI can be a plus or just noise in the workflow of RF design. Which tools
- The PA design optimization using an AI agent loop is an interesting approach. However, the optimization appears to be based solely on circuit-level simulation, with no apparent feedback from layout-related parameters.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `D07`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **4.00 column H avg; min 4; max 4**

### Reviewer remarks
- The objective is clear and feasible for the time frame. Seems to be a good contribution to gLayout if planning to use as base framework.
- Could be a nice add to glayout, parasitics ahead proposal. LLMs are planed to be use for "code free" and "natural lenguage use"; this could reduce the frcition of the tool if the harness is good enough.
- The proposed scope appears achievable within the available schedule. However, the AI-related objectives and deliverables are not clearly articulated.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `D08`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.00 column H avg; min 3; max 3**

### Reviewer remarks
- spice2gds tool proposal. gLayout, gdsfactory, align, and HuggingFace as part of the tool stack. AI optimized flow documented take in considereation PEX, LVS, DRC (similar proposal of this chipaton did not include all of them, from my record this is the 1st one). Is an ambitious project, hard to generalize; participants are planning to test the flow
- Interesting proposal that tries to automate the generation of GDS from spice netlist. Good to see that it combines several tools for automatic generation and that have a framework that seems to be working. By the demo shown seems to be feasible. However, it is important that you can focus in certain designs. Also, I guess you might probably need to
- A good proposal for AI-driven optimization. The use of PEX-derived feedback parameters is particularly valuable, as it enables layout-aware optimization and improves the correlation with final silicon performance.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `D09`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.33 column H avg; min 3; max 4**

### Reviewer remarks
- Hardware accelerator for AI based in RV. Low power focus for edge AI. Proposed design looks feasible and well documented
- The team proposed a low-power, RISC-V-based AI accelerator targeting OCR applications. The hardware design follows a well-established design methodology. However, one important aspect that is not highlighted in the methodology is memory implementation strategy, which often becomes a bottleneck in AI accelerators.
- The proposal has a clear objective: the development of an OCR engine for a RISC-V platform. The scope appears well defined and feasible within the program schedule.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `D10`

**Status:** ⚠️ Not enough reviews

**Review count:** 0 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **2.00 column H avg; min 2; max 2**

### Reviewer remarks
- No reviewer remarks were extracted from the row-2 review comments.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `D11`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.17 column H avg; min 2; max 2.5**
- Feasibility: **2.17 column H avg; min 2; max 2.5**

### Reviewer remarks
- Gloals and tasks seems not to be connected. Goals talk abot RF IC design flow, while tasks and additional project descripton are related to analog in-memory computing systems. Seems that uses devices (memristors) that are not supported by current technology. So it would represent a risk for the actual implementation. Documentation can be improved i
- The team proposed an AI-powered design flow for developing an analog deep-learning accelerator based on in-memory computing using memristors or floating-gate MOSFETs. While the concept is interesting, it is not yet clear whether these technologies can be readily implemented using currently available design flows and fabrication processes. In additi
- I could not clearly understand the relationship between the project goal, the proposed AI-powered RF/analog design flow, and the in-memory analog implementation. The connection between these elements is not sufficiently explained in the proposal.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `D12`

**Status:** ❌ Not approved

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **1.00 column H avg; min 0; max 2**
- Feasibility: **1.00 column H avg; min 0; max 2**

### Reviewer remarks
- The idea is to automatically generate designs using an LLM. The focus is on a design flow based on open-source tools. However, the information is very limited due to the absence of a detailed proposal and insufficient methodology description.
- Specification to RTL AI generator, yet I could not well understand what the goal and merit.

### Approval reason
- Fewer than 3 reviews were submitted.
- At least one Documentation score was 0 or 1.
- At least one Feasibility score was 0 or 1.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `D13`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **2.17 column H avg; min 2; max 2.5**
- Feasibility: **3.17 column H avg; min 3; max 3.5**

### Reviewer remarks
- design looks feasible (assuming external fotodiode), not sure where "AI/LLMs" are involve in this project. Docuemntation can be improved.
- The objective is clear with respect to the circuit to be designed/implemented (threshold detector using analog compartor). However, is missing clarifying where specificly AI/LLM will help the design process. It is just mentioned at the end.
- The target application and project objectives are clearly defined. However, it is not clear how AI/LLM technologies would be incorporated into the design flow, or what specific role they would play in achieving the project’s goals.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `D14`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **4.00 column H avg; min 4; max 4**

### Reviewer remarks
- interesting idea, std cells for neuromorphic circuits based on glayout. Could be a great demostration use-case. Could enable easy re-use of the designed circuits by all the OS community. Documentaion is good, preliminar results (sim level), tapeout looks feasible
- Creating neuromorphic cells is an interesting application for glayout. Good to see you already identified the subblocks that will be implemented using cells already available in glayout. Also good point that you already know what are going to be tapeout.
- The concept of a neuromorphic standard cell implemented with gLayout is unique and innovative. The inclusion of circuit schematics is also a strong point, as it provides a clearer view of the proposed implementation and demonstrates technical maturity.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `D15`

**Status:** ⚠️ Not enough reviews

**Review count:** 2 (minimum required: 3)

### Average scores
- Documentation: **2.00 column H avg; min 2; max 2**
- Feasibility: **2.00 column H avg; min 2; max 2**

### Reviewer remarks
- The proposal attempts to design a reconfigurable multicore SoC based on RISC-V. The multicore SoC configuration is performed using an LLM. The system is targeted to be automatically generated from RTL to GDSII. The idea is good, but it may be difficult to connect and configure all modules without a specially trained LLM model. The deatil Proposal i
- I could not clearly identify the AI/LLM-related contribution of the proposal.

### Approval reason
- Fewer than 3 reviews were submitted.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._

---

<!-- chipathon-2026-review-summary -->
## Schematic Review Summary — `D16`

**Status:** ✅ Approved with comments

**Review count:** 3 (minimum required: 3)

### Average scores
- Documentation: **3.00 column H avg; min 3; max 3**
- Feasibility: **3.33 column H avg; min 3; max 4**

### Reviewer remarks
- nice evaluation case using an open digital IP (opentitan) to test LLMs for power optimziation. However no methods are specified for this intent (pure logic-synthesis optimziation?, static/dinamic power opt?). Metrics to take in consideration should be pre-synthesis and post-synthesis netlist's, this point is not specify in the proposal.
- The proposal aims to strip down OpenTitan for low-power edge deployment using LLM-assisted RTL modification. However, the method lacks clarity on how functional correctness is ensured after modification.
- This appears to be an appropriate application of AI/LLMs. Using AI agents to identify root causes of design issues and search for optimization candidates could provide meaningful improvements to the design process.

### Approval reason
- Minimum review count was met and no blocking documentation or feasibility score was found.

_Generated from row 2 reviewer comments and rows 3-5 scores. Averages are read from column H; individual reviewer scores are used only for min/max and approval checks._
