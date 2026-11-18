# VFL-BRB

## Abstract

Vertical federated learning enables institutions holding complementary measurements from the same patients to collaborate without pooling raw data. However, explaining a joint prediction in terms of rules requires matching antecedents across institutions, and the information exchanged during matching may reveal similarities between patient records. We propose VFL-BRB, a vertically federated belief rule base for explicit inference over distributed antecedents. Each global rule links client-owned antecedent blocks through a shared pseudonymous identifier. Clients retrieve candidate rules using locality-sensitive hashing, with keyed encoding protecting local index addresses. The server aligns candidates, combines local distances to activate global rules, and aggregates their consequent beliefs through evidential reasoning. Five-fold cross-validation on six medical datasets partitioned among five simulated clients yielded mean accuracy of 71.58% and Macro-F1 of 65.34%, showing competitive predictive performance among the ten evaluated vertically federated methods. Class discrimination could be improved on CDC Diabetes with overlapping health profiles and on the small six-class Breast Tissue dataset. Additionally, a separate ablation showed that joint rule matching improved mean accuracy over local prediction fusion by 5.09 percentage points. Hash screening reduced exact rule comparisons with little change in accuracy. A breast tissue case traced how measurements from different clients jointly activated rules and distinguished activation strength from support for the predicted class.

## Code availability

The manuscript is currently under review. The experimental code will be made publicly available in this repository upon acceptance of the paper.
