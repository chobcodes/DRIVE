# Assessing Dice scores when applying MIScnn to DRIVE dataset

Exploratory project to use different combinations of U-Net architectures, loss functions and hyperparameters and assess Dice scores for each model.

## Combinations of architectures and loss functions

The following U-Net architectures are tested: standard, attention, compact, dense, residual

The following loss functions are tested: dice coefficient, soft dice, tversky, focal tversky, symmetric focal, symmetric focal tversky, asymmetric focal, asymmetric focal tversky, symmetric unified focal, asymmetric unified focal

### Dice score table

The below table shows the Dice scores for each model resulting from a combination of U-Net architectures and loss functions. The hyperparameters used can be seen in the script in this repository.

| |standard|attention|compact|dense|residual|
|---|---|---|---|---|---|
|**dice_coefficient_loss**|0.8077|0.8043|0.7922|0.7960|0.7893|
|**dice_soft_loss**|0.8120|0.8111|0.8004|0.8112|0.8122|
|**tversky_loss**|0.8151|0.8156|0.8130|0.8112|0.8037|
|**focal_tversky_loss**|0.8118|0.8106|0.8122|0.8102|0.8113|
|**symmetric_focal_loss**|0.8148|0.8198|0|0|0|
|**symmetric_focal_tversky_loss**|0.8152|0.8017|0.8075|0.8054|0.8072|
|**asymmetric_focal_loss**|0.8030|0.7891|0|0|0|
|**asymmetric_focal_tversky_loss**|0.8077|0.8077|0.8079|0.8100|0.8052|
|**sym_unified_focal_loss**|0.8194|0.8192|0.8149|0.8048|0.8112|
|**asym_unified_focal_loss**|0.8196|0.8202|0.8043|0.7900|0.8068|

In the future, more combinations utilising other U-Net architectures, loss functions and hyperparameters will be assessed.
