## Deployment

### Staging
Staging is something we all know we should do. It solves multiple problems. You get to test things in an environment which is a close to produdction as you can make it. You roll things back from staging not from prod. You are always able to demo new things which aren't completely ready.

#### The reason you don't do staging.
The reason you don't do staging is that it doubles the work required for deployment. Deployment is hard, and often goes wrong, and needs you on full alert. To do this in staging in the same way you do it in produ, would mean doubling the time you spend doing the most painful thing you do. If you didn't do the staging deployment with the same sense of urgency that you do the production deployment (and you never would, because you know it's not production when you do it), small things would go wrong. You would skip over them, and quite soon the staging deployment would either fail completely, or be so far away from production that it wouldn't be valuable any more.

#### Why this shouldn't stop you. 
The wrong way to fix this would be to work harder and harder to do a staging deploy. Make sure you dot every i, roll it back when you would have rolled back the production deploy in the same circumstances. Insist on doing a staging deploy first even when you're doing a firefighting rollout of a hotfix.

In fact, you should consider the staging deploy to be so easy that you don't question whether to do it or not. Doubling the work required for deployment should mean pushing a single button twice instead of once. (Of course, quite soon you should be wrting a script which pushes both buttons for you, and pushing one button to start the script.)

#### Step 1 - QA
Can you instantly check if your app is working correctly after doing the deployment? If not instantly, how long does it take? Can you check by setting one set of tests in motion and waiting for the results? Do you avoid manually checking anything? How much confidence do you have in the results?

The first rule of everything is that you can't be sure that anything works unless you have an automated test which finds out whether it does or not.

