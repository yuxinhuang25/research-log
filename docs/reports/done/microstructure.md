## papers
- **ClusterLOB: enhancing trading strategies by clustering orders in limit order books**
    - Source: Quantitative Finance
    - Link: [Taylor & Francis Online 14697688.2026.2665153](https://www.tandfonline.com/doi/pdf/10.1080/14697688.2026.2665153)
    - Tags:  #LOB #OFI #clustering #MBO #alpha_short_horizon
    - Note:
        - One-line idea:
        Cluster orders to purify OFI signal

        - Structure:
        order-level features → K-means → cluster OFI → return prediction

        - Signal:
        cluster-specific OFI

        - Features:
            - V (volume at price level)
            - Tm (time since last mid-price change)
            - T1 (time since first order at price)
            - T' (inter-arrival time)
            - SBS (same book side depth)
            - OBS (opposite book side depth)

        - Method:
        K-means++ clustering on MBO data

        - Label:
        FRNB / FREB (30-min future returns)

        - Alpha idea:
        By clustering order behavior, OFI becomes less noisy → improves short-term return predictability

        - Memory hook:
        cluster first → aggregate OFI

        - A-share mapping:
            - Level2 order data can replicate this idea
            - can extend to cancel/add/trade decomposition
            - useful for intraday / short-horizon alpha