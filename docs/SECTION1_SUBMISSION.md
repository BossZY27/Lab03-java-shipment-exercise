# Section 1 Submission Notes

## Assignment

Java OOP exercise: calculate shipment cost by weight and shipment type, then print all shipments and the total cost.

Rates:

| Type | Rate |
| --- | ---: |
| STANDARD | 40 baht/kg |
| EXPRESS | 100 baht/kg |

## Selected Section

Section 1: SpeedEx Logistics

Files kept for submission:

- `src/main/java/com/example/ShipmentSection1_Exercise.java`
- `src/test/java/com/example/ShipmentTest_Section1.java`
- `expected-output/ExpectedOutput_Section1.md`

Section 2, Section 3, and Section 4 files were removed according to the assignment instructions.

## Fixed Items

- Added missing `STANDARD` shipment type.
- Fixed the `Shipment` constructor parameter order to `(trackingNumber, weightKg, type)`.
- Corrected shipment rates:
  - `STANDARD_RATE = 40.0`
  - `EXPRESS_RATE = 100.0`
- Completed `toString()` output formatting.
- Initialized the `shipments` list in `ShippingCompany`.
- Implemented total-cost calculation by summing every shipment.
- Completed summary printing with shipment rows and final total.
- Added `package com.example;` so the Maven/JUnit test can access the main classes.

## Expected Program Output

```text
========================================
  บริษัท        : SpeedEx Logistics
  จำนวน Shipment : 5 รายการ
========================================
[TH001]  3.00 กก. | STANDARD |    120.00 บาท
[TH002]  1.50 กก. | EXPRESS  |    150.00 บาท
[TH003]  5.00 กก. | STANDARD |    200.00 บาท
[TH004]  2.00 กก. | EXPRESS  |    200.00 บาท
[TH005] 10.00 กก. | STANDARD |    400.00 บาท
----------------------------------------
  ยอดรวมทั้งหมด : 1,070.00 บาท
========================================
```

## How To Run

Open the project in Eclipse or VS Code, then run:

`src/main/java/com/example/ShipmentSection1_Exercise.java`

For Maven test:

```bash
mvn -Dtest=ShipmentTest_Section1 test
```

Expected Maven result:

```text
[INFO] Tests run: 7, Failures: 0, Errors: 0, Skipped: 0
[INFO] BUILD SUCCESS
```

## Screenshots Required By Assignment

Create a `screenshots/` folder and add these two images:

- `screenshots/program_output.png`: program output from Eclipse or VS Code console.
- `screenshots/mvn_test_result.png`: Maven test result showing `BUILD SUCCESS`, `Failures: 0`, and `Errors: 0`.

After adding screenshots:

```bash
git add screenshots/
git commit -m "screenshot: add section 1 results"
git push origin main
```

## Submission Link

Submit this repository link:

https://github.com/BossZY27/Lab03-java-shipment-exercise
