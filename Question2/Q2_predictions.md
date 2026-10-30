# Q2 predictions

## Q2.5 (written before running the tests in "Testing the Baseline")

I think Model A will perform reasonably well with mirrored digits, but the results might not be perfect. The reason is that mirroring doesn't really change how the digits move. They still follow the same straight-line motion and bounce off the boundaries, just like in the training data. Also, from Figure 1, we can see that the model has already seen digits moving in different directions. However, the problem is that mirrored digits look different from normal digits. For example, a reversed 3 or 5 would look unfamiliar to the model. So, I expect the prediction error to increase slightly, and the generated digits might become a bit blurry.

For rotation, I think the model will struggle more compared to mirroring. Even though the movement stays the same, rotating the digits changes their appearance quite a lot. Since the model hasn't learned these rotated shapes properly, I think it might start losing the digit shapes more quickly.

For speed, Model A can transfer information up to around 8 pixels per step. At normal speed (1×), the digits move about 3.3 pixels per frame, while at 2× speed, they move around 6.6 pixels. Both are within the model's limit, so I think it should still work at 2×, although the predictions might not be as accurate. But at 3× speed, the digits move around 10 pixels per frame, which is beyond what the model can handle in one step. So, I expect the model to struggle significantly at 3×, and the digits might become blurry, stop moving properly, or even disappear.
