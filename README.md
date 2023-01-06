# Assessing Dice scores when applying MIScnn to DRIVE dataset

Exploratory project to use different combinations of U-Net architectures, loss functions and hyperparameters and assess Dice scores for each model.

## Combinations of architectures and loss functions

The following U-Net architectures are tested: standard, attention, compact, dense, residual

The following loss functions are tested: dice coefficient, soft dice, tversky, focal tversky, symmetric focal, symmetric focal tversky, asymmetric focal, asymmetric focal tversky, symmetric unified focal, asymmetric unified focal

| |standard|attention|compact|dense|residual|
|---|---|---|---|---|---|
|**dice_coefficient_loss**|0.8077|||||
|**dice_soft_loss**|0.8120|||||
|**tversky_loss**|0.8151|||||
|**focal_tversky_loss**|0.8118|||||
|**symmetric_focal_loss**||||||
|**symmetric_focal_tversky_loss**|0.8152|||||
|**asymmetric_focal_loss**|0.8030|||||
|**asymmetric_focal_tversky_loss**|0.8077|||||
|**sym_unified_focal_loss**|0.8194|||||
|**asym_unified_focal_loss**|0.8196|||||
