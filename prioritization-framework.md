# Prioritization Framework
To better intake and prioritize the topics for interoperability the working group has created a questionnaire tailored to the topic of DASH/HLS interoperability. 

Each proposed topic must be a standalone use-case / component of streaming allowing for the questions to be unambiguously answered relative to the topic. The questionnaire results in a prioritization scoring that is used to stack rank proposed work.

**Note:** While the prioritization provides a guiding framework, the working group ultimately decides the prioritization of each item. The working group should document and communicate any prioritization different from the scoring provided by the framework.

# Questionnaire
The questionnaire is broken up into three main litmus tests with sub-considerations.

## Does the feature relate to an industry streaming use-case?
The purpose of this litmus test is to establish that the feature / functionality relates to general industry needs and warrants the attention of the working group. 

| Classification | Meaning |
|--------------|---------|
| Yes | The feature is directly related to an industry use-case and should be generally considered.
| No | The feature is not directly related to an industry use-case, but may still warrant consideration if time allows.

This sub-considerations of this test are used to establish industry recognition of the use-case.

### What is the commonality of the case?

| Classification | Score | Meaning |
|----------------|-------|---------|
| Uncommon | 0 | The streaming use-case is not commonly found across the streaming industry.
| Common | 1 | The streaming use-case is generally found across the streaming industry.
| Very Common | 2| The streaming use-case is so common that it's unlikely to not find it across the streaming industry.

### Is this an established or emerging practice?

| Classification | Score | Meaning |
|----------------|-------|---------|
| Declining | 0 | The use-case is seeing a reduction of adoption.
| Established | 1 | The use-case adoption has normalized at a percentage of the streaming industry.
| Emerging | 2 | The use-case is seeing growing adoption within the streaming industry.

## Does this feature have related mechanisms in both DASH and HLS?
The purpose of this litmus test is to establish a baseline understanding of fore-running work across the DASH and HLS specifications and any details around known issues or missing constraints to assist the working groups efforts.

### What is the maturity of support in both specification?

| Classification | Score | Meaning |
|----------------|-------|---------|
| Immature Both | 0 | The feature is not present or very recently available in both the DASH/HLS specifications.
| Mature Single | 1 | The feature is considered mature / well-established in one specification, the specification should be noted.
| Mature Both | 2 | The features is considered mature / well-establish in both specifications. Note this does not imply feature parity or interoperability, just existence.

### What is the maturity of implementation support for both specifications?

| Classification | Score | Meaning |
|----------------|-------|---------|
| Immature Both | 0 | The feature is not present or incomplete in major implementations of the DASH/HLS specifications.
| Mature Single | 1 | The feature is present / complete in major implementations of one of the specifications, the specification should be noted.
| Mature Both | 2 | The feature is present / complete in major implementations of both of the specifications.

### Are there known interoperability issues in both specifications?

| Classification | Score | Meaning |
|----------------|-------|---------|
| No | 0 | There are no known interoperability issues and none are believed to be discovered
| Potentially | 1 | There are presently no known interoperability issues, but there could be discovered with further investigation.
| Yes | 2 | There are known interoperability issues that have to be addressed.

### Has anyone implemented an interoperable solution for this?

| Classification | Score | Meaning |
|----------------|-------|---------|
| No | 0 | There are no known implementations that serve DASH and HLS interoperably
| Potentially | 1 | There are no well-known implementations that serve DASH and HLS interoperably but there are candidates that may have working solutions. Potentially working examples should be noted for reference.
| Yes | 2 | There are well-known implementations that serve DASH and HLS. Implementations should be noted for reference.

### Is the feature missing in a specification with open proposals for it?

| Classification | Score | Meaning |
|----------------|-------|---------|
| No | 0 | The feature already exists in both specifications, irrespective of maturity status.
| Yes Single | 1 | The feature does not exist in one specification and a proposal exists for its inclusion.
| Yes Both | 2 | The feature does not exist in either specification and proposals exist for its inclusion in both.

## Has the industry defined de-facto mechanisms not present in both DASH and/or HLS?
The purpose of this litmus test is to discover if there are potential de-facto solutions in the industry that need to be better specified and shepherded towards interoperability by the working group. This test may not be relevant to all feature considerations.

### Why was functionality defined outside of the main specifications?

| Classification | Score | Meaning |
|----------------|-------|---------|
| Unknown / N/A  | 0 | The history of the external standardization is not known or the feature has not been standardized anywhere.
| Spec Invalid | 1 | The feature was proposed but considered invalid in the context of the specification. Known details should be noted.
| Industry Desire | 2 | The feature was standardized by members of the industry prior to the main standards being able to act on them.

### Has the functionality been standardized elsewhere? (DASH-IF, CTA, SVA, etc)

| Classification | Score | Meaning |
|----------------|-------|---------|
| No | 0 | The functionality is not standardized anywhere
| Yes | 1 | The functionality is standardized somewhere, the location should be noted

### Is the functionality proprietary or openly developed?

| Classification | Score | Meaning |
|----------------|-------|---------|
| Proprietary | 0 | The functionality was developed by an entity in private and may have rights holders. Any known holders / owners should be noted.
| Open | 1 | The functionality was developed with an open methodology either from the start or after initial contribution from a private entity.

### Could the functionality be incorporated into specifications with evangelism?

| Classification | Score | Meaning |
|----------------|-------|---------|
| No | 0 | It is unlikely for the main DASH/HLS specifications to adopt the functionality even with proper evangelism
| Yes | 1 | It is likely for the main DASH/HLS specifications to adopt the functionality with proper evangelism

# Prioritization Score
The total prioritization score is the sum of the scores of each main litmus test. The score of a litmus test is the sum of it's sub-considerations if the test is relevant or 0 if the test is not relevant.

The goals of the scoring are to identify topics with high levels of industry interest and/or potential industry impact. This is represented by the score depicted above for each answer classification.

# Questionnaire Markdown Form

Contained here is a markdown version of the questionnaire that can be copied into any issue and answered, the working group will add in the scoring details once reviewed.

```
| Question | Answer |
|----------|--------|
| Does the feature relate to an industry streaming use-case? | Yes, No |
| - What is the commonality of this use-case? | Uncommon, Common, Very Common |
| - Is this an established or emerging practice? | Declining, Established, Emerging |
| Does this feature have related mechanisms in both DASH and HLS? | Yes, No |
| - What is the maturity of support in both specifications? | Immature Both, Mature Single, Mature Both |
| - What is the maturity of implementation support for both specifications? | Immature Both, Mature Single, Mature Both |
| - Are there known interoperability issues in both specifications? | No, Potentially, Yes |
| - Has anyone implemented an interoperable solution for this? | No, Potentially, Yes |
| - Is the feature missing in a specification with open proposals for it? | No, Yes Single, Yes Both | 
| Has the industry defined de-facto mechanisms not present in both DASH and/or HLS? | Yes, No |
| - Why was the functionality defined outside of the main specifications? | Unknown / N/A, Spec Invalid, Industry Desire |
| - Has the functionality been standardized elsewhere? (DASH-IF, CTA, SVA, etc) | No, Yes |
| - Is the functionality proprietary or openly developed? | Proprietary, Open |
| - Could the functionality be incorporated into specifications with evangelism? | No, Yes |
```

Rendered view:

| Question | Answer |
|----------|--------|
| Does the feature relate to an industry streaming use-case? | Yes, No |
| - What is the commonality of this use-case? | Uncommon, Common, Very Common |
| - Is this an established or emerging practice? | Declining, Established, Emerging |
| Does this feature have related mechanisms in both DASH and HLS? | Yes, No |
| - What is the maturity of support in both specifications? | Immature Both, Mature Single, Mature Both |
| - What is the maturity of implementation support for both specifications? | Immature Both, Mature Single, Mature Both |
| - Are there known interoperability issues in both specifications? | No, Potentially, Yes |
| - Has anyone implemented an interoperable solution for this? | No, Potentially, Yes |
| - Is the feature missing in a specification with open proposals for it? | No, Yes Single, Yes Both | 
| Has the industry defined de-facto mechanisms not present in both DASH and/or HLS? | Yes, No |
| - Why was the functionality defined outside of the main specifications? | Unknown / N/A, Spec Invalid, Industry Desire |
| - Has the functionality been standardized elsewhere? (DASH-IF, CTA, SVA, etc) | No, Yes |
| - Is the functionality proprietary or openly developed? | Proprietary, Open |
| - Could the functionality be incorporated into specifications with evangelism? | No, Yes |
