---
# This is contract data in the yaml format.
# This is a change I really can do!
author: "Leif Arne Bakker"
businessRegistrationNoPurchaser: "233121322"
businessRegistrationNoSeller: "43543345345"
businessRegistrationNoTargetCompany: "387634222"

# The percentage depends on, inter alia, the amount of the loss carry forward.
compForDiffPropValAndTaxDeprInNOK: "200.230"

date: "02.03.18"
closingDate:"12.04.18"
landNo: "2534534-435"
lossCarryForwardInPercent: "2.5"
latePaymentIneterstRateInPercent:"3.3"
municipality: "Oslo"
purchasePriceInNOK: "12.344.000"
estimatedPurchasePriceInNOK: "11.100.000"
settlementAmountInNOK:"12.500.000"
creditor: "Creditor AS"
debitor: "Debtor AS"
fixedConsiderationForDeferredTaxBenefitInNOK: "12.233"
fixedDeductionForDeferredTaxInNOK: "10.212"

subsidiary_1_name: "Kroken 4 AS"
subsidiary_1_regNo: "1277231771"
subsidiary_2_name: "Alna 12 AS"
subsidiary_2_regNo: "127672167"
theCompany: "Brugata 12 AS"
theEstateAgency: "Eiendomsmagnaten AS"
thePurchaser: "Bruube AS"
theSeller: "Avenir AS"
titleHoldingCompany: "The Title Company AS"
titleHoldingCompanyOrgNo: "1723872372"
titleNo: "82772"

# If subsidiary set this to 'Group' otherwise use 'Company'
companyOrGroup: "The CompanyGroup AS"

# Optional Clauses
ifSubsidiary: true
ifUseTitleHoldingCompany: true
ifFixedConsiderationForDeferredTaxBenefit: true
ifFixedDeductionForDeferredTax: true

# Footnote 9
ifCompanyBankLoansNotRepaid: true

# Footnote 11
ifIncludeSellerLoanClause: true
sellerLoanAmountInNOK: "NOK 4.100.000"

# Footnote 12 & 13. Only one option can be true, the others false.
ifSimplifiedAuditOfBalanceSheet: true
ifStandardAuditOfBalanceSheet: false
ifThoroughAuditOfBalanceSheet: false
companyAccountantName: "PWC"

# Footnote 15 Only one can be true
ifStandardClosingConditions: false
ifUncertainClosingConditions: true
numberOfClosingDaysWhenUncertainConditions: 14

# Footnote 16 If seller require name change
ifSellerRequireNameChange: true
designationToRemove: "The NameToRemove"

##Footnote 18
ifUseExtendedClauseDueToCompetitionAct: true

# Structured Headers
level-1: "### 1."
level-2: "#### pre 1."
level-3: "(a)"
level-4: "(a)"
level-5: "(a)"

# Properties
no-indent: "l., ll."
no-reset: "l."
level-style: "l."

---

---
output: word_document
---
![Logo](assets/images/logo.png)

STANDARD ESTATE AGENCY TERMS, OCTOBER 2015, FOR THE SALE AND PURCHASE OF A PRIVATE LIMITED LIABILITY COMPANY, WITHOUT CLOSING AGENT. Draft A **{{date}}** from **{{theEstateAgency}}** by **{{author}}**. **{{theEstateAgency}}** has examined neither issues relating to direct or indirect taxes, nor accounting issues. It is recommended that these be evaluated by the advisors of the parties or by their auditors. The agreement is concluded when signed by the seller and the purchaser.

# SALE AND PURCHASE AGREEMENT
**between {{theSeller}} and {{thePurchaser}} relating to the sale and purchase of the shares of {{theCompany}}.**


---

```

l. THE PARTIES AND THE PROPERTY

**{{theSeller}}**, business registration no. **{{businessRegistrationNoSeller}}**, (the Seller) is the owner of 100% of the shares (the Shares) of the **{{theCompany}}**, business registration no. **{{businessRegistrationNoTargetCompany}}**, (the Company).

The Seller and **{{thePurchaser}}**, business registration no. **{{businessRegistrationNoPurchaser}}**, (the Purchaser) agree that the Shares shall be transferred from the Seller to the Purchaser on the terms set out in this agreement. [{{ifSubsidiary}} The Company owns all shares of **{{subsidiary_1_name}}**, business registration no. **{{subsidiary_1_regNo}}**, and **{{subsidiary_2_name}}**, business registration no. **{{subsidiary_2_regNo}}**, hereinafter jointly referred to, together with the Company, as the Group." ]

The **{{theCompany}}** is the owner of land no. **{{landNo}}**, title no. **{{titleNo}}**, together with its existing buildings and facilities in the municipality of **{{municipality}}** (the Property).

[{{ifUseTitleHoldingCompany}} The **{{theCompany}}** is also the owner of all shares of **{{titleHoldingCompany}}** AS, business registration no. **{{titleHoldingCompanyOrgNo}}**, (the Title-Holding Company), which is registered as holding title to the Property in the Register of Land Titles and Land Charges."]


l.	THE PURCHASE PRICE

ll.	The Property Value and calculation of the Purchase Price

The Purchase Price for the Shares (the Purchase Price) shall be:

lll.	NOK **{{purchasePriceInNOK}}**, which represents an agreed, fixed value for the Property (the Property Value);
plus:

lll.	the cash and receivables on the balance sheet of the **{{companyOrGroup}}**;

lll.	**{{lossCarryForwardInPercent}}%**  of any loss carry forward (until and including the date of Closing);

[{{ifFixedConsiderationForDeferredTaxBenefit}} lll. NOK **{{fixedConsiderationForDeferredTaxBenefitInNOK}}**, which represents an agreed, fixed consideration in respect of deferred tax benefit comprising loss in the gain/loss account.]
minus:

lll.	all liabilities on the balance sheet of the **{{companyOrGroup}}**(including the Loans as defined in Clause 2.2) with the exception of deferred tax and provision for bad debts;  and

[{{ifFixedDeductionForDeferredTax}} lll. NOK **{{fixedDeductionForDeferredTaxInNOK}}**, which represents an agreed, fixed deduction in respect of deferred tax comprising gain in the gain/loss account; and]

lll.	NOK **{{compForDiffPropValAndTaxDeprInNOK}}**, which represents an agreed, fixed amount to compensate for the difference between the Property Value (less the agreed value of the land) and the basis for tax depreciation of the Property.

ll. |2.2|The Estimated Balance Sheet and the Estimated Purchase Price[{{ifCompanyBankLoansNotRepaid}}, as well as repayment of the Loans]

The Purchase Price payable by the Purchaser upon Closing (the Estimated Purchase Price), shall be determined on the basis of a balance sheet for the Company as it is expected to be as per Closing (the Estimated Balance Sheet). The Estimated Balance Sheet shall be prepared in accordance with generally accepted accounting principles, consistently applied, and otherwise as follows:

lll.	Expected profit/loss after tax until and including the date of Closing shall be included.

[{{ifCompanyBankLoansNotRepaid}} lll. The liabilities of the Company shall include all income/costs, including any premium or discount and any costs incurred upon the discharge of swap agreements, that will arise upon repayment of the Company's bank loans (in aggregate the Loans) upon Closing.]

lll.	Payable tax and deferred tax benefits shall reflect[{{ifCompanyBankLoansNotRepaid}}i) the income/costs that will arise upon repayment of the Loans, and ii)] the Company's tax depreciation and entries from the gain/loss account, etc., in the sales year, allocated on the basis of the period of ownership during the sales year, calculated as the number of days of ownership, with the date of Closing being allocated to the Seller.

lll.	Deferred tax benefits and deferred tax shall not be recorded as one net amount, but as two gross items under assets and liabilities.

Appendix 3 contains an Estimated Balance Sheet prepared by the accountant of the Company, and a calculation of the Estimated Purchase Price, which is estimated at NOK **{{estimatedPurchasePriceInNOK}}**.

[{{ifCompanyBankLoansNotRepaid}} The Seller shall, no later than five days before Closing, submit to the Purchaser statements of outstanding debt from the bank(s) of the Company, showing the exact amount of the Loans as per Closing. The Seller shall, at the same time, submit an updated calculation of the Estimated Purchase Price in which the Loans are updated with the correct amount, but without changes having been made to the other entries, including payable tax and deferred tax benefit. If Closing is delayed for any reason, the Seller shall, without undue delay, provide a new statement of outstanding debt and a new calculation of the Estimated Purchase Price as per the date of Closing.]

The Purchaser shall pay the Estimated Purchase Price upon Closing [{{ifCompanyBankLoansNotRepaid}} and repay the Loans in the amounts set out in the statement of outstanding debt.]

[{{ifIncludeSellerLoanClause}} Furthermore, the Purchaser shall, at the same time and on behalf of the Company, repay the debt outstanding from the Company to the Seller (the Seller Loan), which is in the amount of **{{sellerLoanAmountInNOK}}**, including accrued interest, as per Closing.]

The Seller and the Company hereby confirm that any claim between the **{{companyOrGroup}}** and the Seller or other companies in the same group as the Seller, is settled with final effect after **{{creditor}}** has received NOK **{{settlementAmountInNOK}}** from **{{debitor}}** upon Closing], and that any claim omitted in the Revised Balance Sheet is waived in its entirety with effect from Closing.


ll.	The Revised Balance Sheet and the Revised Purchase Price

The Seller shall send the following to the Purchaser no later than 45 days after Closing:

lll.	An updated balance sheet as per Closing (the Revised Balance Sheet), prepared pursuant to the same principles as the Estimated Balance Sheet, cf. Clause |2.2| (provided, however, that any arrangements made by the **{{companyOrGroup}}** on the date of Closing after the Purchaser has taken delivery of the Shares shall be disregarded) and approved and signed by those who served as Directors of the **{{companyOrGroup}}** immediately prior to Closing;

lll.	[{{ifStandardAuditOfBalanceSheet}}A certification from an auditor appointed by the Seller, to the effect that such auditor has conducted a simplified audit check of the Revised Balance Sheet; and][{{ifSimplifiedAuditOfBalanceSheet}}A certification from **{{companyAccountantName}}**, to the effect that he has conducted a simplified check of the Revised Balance Sheet; and][{{ifThoroughAuditOfBalanceSheet}}A certification from the auditors to the effect that the Revised Balance Sheet has been prepared and audited in conformity with the provisions governing annual financial statements; and]

lll.	A calculation of the Purchase Price (the Revised Purchase Price) on the basis of the Revised Balance Sheet.

The Purchaser may, no later than 14 days  after receiving the Revised Balance Sheet and the calculation of the Revised Purchase Price (hereinafter jointly referred to as the Purchase Price Calculation), notify the Seller in writing if he has objections to the Purchase Price Calculation. If the Purchaser fails to invoke any objection within the aforementioned time limit, the Purchase Price Calculation prepared by the Seller shall become final and binding on the parties.

If the Purchaser invokes an objection against the Purchase Price Calculation within the aforementioned time limit and the parties do not reach agreement within an additional 14 days, an independent chartered accountant, jointly appointed and paid for by the parties, shall determine the Purchase Price Calculation with final and binding effect for the parties. The outcome of such determination shall be submitted no later than 14 days after the chartered accountant has been appointed.

If the parties do not reach agreement as to which chartered account should be used, either of the parties may require that such chartered accountant be appointed by the Chairperson of the Norwegian Financial Services Association (FNH). To the extent that the chartered accountant needs to take a view on legal issues for purposes of his or her determination, such determination shall be deemed to constitute an arbitral award and shall be governed by the provisions of the Arbitration Act to the extent that they do not conflict with this provision, and such award may only be set aside by the ordinary courts of law via legal action as mentioned in Section 42 of the Arbitration Act. The chartered accountant shall be made aware of this, as well as of the final and binding effect the chartered accountant's decision will have for the parties. The chartered accountant shall be entitled to appoint, at his or her own discretion and for the account of the parties, an independent lawyer to perform a legal assessment of the objection, in which case such assessment shall be submitted to both parties for commenting prior to a decision being made. The parties and the Company shall grant the chartered accountant access to all information the chartered accountant many request with regard to the Company.

If the Revised Purchase Price deviates from the Estimated Purchase Price;

a) any positive difference shall be paid by the Purchaser to an account specified by the Seller; and

b) any negative difference shall be paid by the Seller to an account specified by the Purchaser.

The difference shall be paid no later than 14 days after the Purchase Price Calculation has been determined with final effect, with the addition of **{{latePaymentIneterstRateInPercent}}%** interest p.a. as from Closing until payment is made, provided, however, that late payment interest pursuant to the Late Payment Interest Act shall accrue after the due date.

The fact that the Purchase Price Calculation is final and binding shall not prevent the Purchaser from invoking claims as the result of breach of any other provision of this agreement.

ll.	Late payment

If the Estimated Purchase Price or any other amount outstanding under this agreement is not paid by the due date, the debtor shall pay late payment interest pursuant to the Late Payment Interest Act from the due date until payment is made.


l.	CLOSING, RISK TRANSFER AND SETTLEMENT

[{{ifStandardClosingConditions}}]
The Purchaser shall take delivery of the Shares at 12:00 noon on **{{closingDate}}** (Closing).

[{{ifUncertainClosingConditions}}Closing shall take place **{{numberOfClosingDaysWhenUncertainConditions}}** banking days after all conditions in Clauses 4.1 and 4.2 have been satisfied or waived.]

The Purchaser shall, from that point in time, assume the risk that any circumstances may arise that would amount to defects or breaches of the warranties made as per Closing.

Closing shall take place in accordance with the closing agreement in Appendix 8, and the Seller, the Purchaser and the Company hereby undertake to perform their respective duties under the closing agreement. [{{ifSellerRequireNameChange}} The Purchaser shall change the name of the Company no later than 1 month after Closing such as to remove the designation "{{designationToRemove}}". Neither the Purchaser, nor the Company, shall be permitted to use the designation "designationToRemove" in marketing or otherwise after Closing."] The Seller shall ensure that the Company performs its duties under the closing agreement.

l.	CONDITIONS PRECEDENT TO CLOSING

ll.	Conditions on the part of the Purchaser

[{{ifUseExtendedClauseDueToCompetitionAct}}The acquisition of the Shares by the Purchaser has been cleared by the Norwegian Competition Authority either by the Authority stating that the examination of the transaction by the Authority has been completed, or by the Authority refraining from giving notice of further examination within the time limits stipulated in the Competition Act.]





```
