# GAS_BIZ_Diesel

GREET
    \- Guest First Name
    \- Reason for Visit
ALU_DISCOVER
    \- Tenure_Appreciation
    \- Business_Internet
    \- Discounts
    \- StrategicOffers
    \- DeviceTypes
    \- AAL_&_eSIM
    \
    \- OldPlanPrice
        \- Line01 = ["$"]
        \- Line02 = ["$"]
        \- Line03 = ["$"]
        \- Line04 = ["$"]
        \- Line05 = ["$"]
     \- NewPlanPrice
        \- Line01 = ["$"]
        \- Line02 = ["$"]
        \- Line03 = ["$"]
        \- Line04 = ["$"]
        \- Line05 = ["$"]
     \- Discounts
        \- Line01 = ["$"]
        \- Line02 = ["$"]
        \- Line03 = ["$"]
        \- Line04 = ["$"]
        \- Line05 = ["$"]
     \- DevicePayment
        \- Line01 = ["$"]
        \- Line02 = ["$"]
        \- Line03 = ["$"]
        \- Line04 = ["$"]
        \- Line05 = ["$"]
     \- Buyout_/_Trade
        \- Line01 = ["$"]
        \- Line02 = ["$"]
        \- Line03 = ["$"]
        \- Line04 = ["$"]
        \- Line05 = ["$"]
BIZ_PERKS
    \- Reveal_/_Fleet
    \- OneTalk
    \- MobilePotection
    \- 2_Person_Integrity_SignOff
SAFE_WALK
    \- Demo3_Devices
    \- Show_5_Accessories
CLOSE
    \- B360_Quote = []
    \- RTG = []
    \- RQ_Invoice# = []
    \- Lead_Submitted = []
    \- RIS_Education = []
    \- Converted_Contro_&_Products = []


MyBizPlan
    \- infoData
        \- infoData01 = ["$5/mo_Military_Discount"]
    \- Lines
        \- overall
            \- Features
                = [
                    "Unlimited Talk, text, and data 5GB Mobile Hotspot, Standard Def Video, Call Filter, Canada & Mexico",
                ]
        \- if(line === 1) {
            if (AutoPay === true) => ["$65"]
            if (AutoPay === false) => ["$70"]
        }
        |
        \- if (lines === 2) {
            if (AutoPay === true) => ["$55"]
            if (AutoPay === false) => ["$60"]
        }
        |
        \- if (lines === 3) {
            if (AutoPay === true) => ["$40"]
            if (AutoPay === false) => ["$45"]
        }
        |
        \- if (lines === 4) {
            if (AutoPay === true) => ["$34"]
            if (AutoPay === false) => ["$39"]
        }
        |
        \- if (lines >== 5) {
            if (AutoPay === true) => ["$55"]
            if (AutoPay === false) => ["$60"]
        }
BusinessUnlimitedPlans
    \- if ("Legacy", "$55", true) {
        item01: ["25GB_PremiumData","15GB_MobileHotspot","5G_UltraWideband"]
    },
    |
    \- if ("Legacy", "$50", true) {
        item02: ["22GB_PremiumData","10GB_MobileHotspot","5G_Nationwide"]
    },
    |
    \- if ("Legacy", "$40", true) {
        item03: ["5mbps_MaxSpeed","15GB_MobileHotspot","DevicePayment_req'd"]
    },
    \- if ("BasicPhone", "$30", true) {
        item01: ["UnlimitedData","No_Mobile_Hotspot",""]
    },
BusinessAddOns
    \- [false] - VMISSecurity - [$0]
    \- [false] - Unlimited_Cloud_Storage - [$0]
    \- [false] - International_Connectivity - [$0]
    \- [false] - Premium_Network_Exp - [$0]
    \- [false] - Google_Workspace - [$0]
    \- [false] - International_Long_Distance - [$0]
    \- [false] - Business_Mobile_Secure+ - [$0]
    \- [false] - 50GB_Mobile_Hotspot - [$0]