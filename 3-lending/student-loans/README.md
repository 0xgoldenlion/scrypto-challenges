# RadEDU Student Loans

## How to try out this project

The src folder contains the Scrypto source.

To run the project, navigate to the RadEDU Student Loan - Front End folder and run:
npm install && npm run start

You must install the PTE browser extension. More info here: https://docs.radixdlt.com/main/scrypto/public-test-environment/pte-getting-started.html

## About

This project seeks to explore what a Student Loan protocol might look like on Radix. Drawing from Scrypto examples provided by the Radix team, this project is a simple lending protocol with 4 features:

1) **Interest rate dependent on expected income:** Loan interest rate is determined by projected income based on the major chosen by the student. For example, we might expect an engineer to earn more after graduation than a Fine Arts major. The engineer major in this case will receive a higher interest rate. 

2) **Soulbound token:** When a user is registered, a soulbound token is used by applying the following to a fungible resource:
**.restrict_withdraw( rule!(deny_all), LOCKED )**

Just as in traditional student loans, this mechanism helps to emulate (for better or for worse) the fact that bankruptcy does not forgive student loans in the United States.

3) If the student is unemployed or cannot generate income, we can change the interest rate to 0% in a forbearance arrangement.

4) It uses the Radix PTE SDK in order to be used as a simple dApp.


## License

The Radix Official Examples code is released under Radix Modified MIT License.

    Copyright 2024 Radix Publishing Ltd

    Permission is hereby granted, free of charge, to any person obtaining a copy of
    this software and associated documentation files (the "Software"), to deal in
    the Software for non-production informational and educational purposes without
    restriction, including without limitation the rights to use, copy, modify,
    merge, publish, distribute, sublicense, and to permit persons to whom the
    Software is furnished to do so, subject to the following conditions:

    This notice shall be included in all copies or substantial portions of the
    Software.

    THE SOFTWARE HAS BEEN CREATED AND IS PROVIDED FOR NON-PRODUCTION, INFORMATIONAL
    AND EDUCATIONAL PURPOSES ONLY.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
    FOR A PARTICULAR PURPOSE, ERROR-FREE PERFORMANCE AND NONINFRINGEMENT. IN NO
    EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES,
    COSTS OR OTHER LIABILITY OF ANY NATURE WHATSOEVER, WHETHER IN AN ACTION OF
    CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
    SOFTWARE OR THE USE, MISUSE OR OTHER DEALINGS IN THE SOFTWARE. THE AUTHORS SHALL
    OWE NO DUTY OF CARE OR FIDUCIARY DUTIES TO USERS OF THE SOFTWARE.

