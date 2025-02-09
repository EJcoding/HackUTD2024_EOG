# EOG Resources - HackUTD: RippleEffect

# Hydrate Detection Challenge 🧊

## Challenge Statement 🏋️
Imagine you are a lease operator at EOG, tasked with ensuring optimal production from a group of wells. One of the challenges you face is the formation of hydrates (ice-like solids made of frozen natural gas) that can form inside pipelines and block the injection of gas. This blockage can significantly reduce oil production and potentially lead to costly well shutdowns.
 
As a lease operator, your goal is to efficiently monitor these wells and quickly identify any instances of hydrate formation. You have access to data streams that include the current gas injection volume, target gas injection volume, and valve open percentage. Your challenge is to develop a solution that makes it easy and quick to detect when a hydrate occurs, allowing the lease operator to take swift action to minimize production loss.

## Additional Information 📝
### What does a hydrate actually look like?
### How does a hydrate form and why does it cause production loss?
  - Oil wells produce more oil when gas is injected into them. High-pressure gas is delivered to a well from a compressor station via a pipeline. This pipeline is underground for the most part but rises above ground before it reaches a well to allow for maintenance when needed. However, sometimes the change in temperature and pressure that occurs at the riser can cause a hydrate to form. The formation of hydrates is not a desirable phenomenon as it blocks gas from being injected into the well, which in turn decreases oil production and could potentially cause the well to be shut in, costing the company millions of dollars.

            ---------------=-----========---------------------=--------
                        |         Valve     ICEPLUG
            ---------------=-----========------------------------------

### What are the data streams available to us and what do they mean?
 - **Inj Gas Meter Volume Instantaneous**: This stream represents the actual volume of gas being injected into the well at the given timestamp.
- **Inj Gas Meter Volume Setpoint**: This stream represents the target or desired volume of gas to be injected into the well for optimal production. 
- **Inj Gas Valve Percent Open**: This stream represents the percentage that the valve controlling the gas injection volume is open at a given timestamp. 0% indicates that the valve is fully closed and 100% indicates that the valve is fully open. The valve is used to control the amount of gas flowing into a well and is automatically adjusted to meet the gas injection volume setpoint (think of this as the gas pedal in your car).
