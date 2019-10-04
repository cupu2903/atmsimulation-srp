# atmsimulation-srp
This is the same study case with atmsimulation repository. so each entity have their own responsibility. For further, the rest api still can be used for another platform

# Short Summary

In order to prevent a massive change that have been built before in study case 3. I choose to keep the Rest API in single module independent, so it can be used for another platform. Such as if we need to built ATM Simulation in Android or iOS, they can communicate with ATM Simulation REST-API seamlessly.

Regarding to security concern, I prefer to implement Json Web Token with Bearer in Header. Since JWT consists of source address, roles and privileges, expired period, I think that&#39;s fairly enough to authorized the message.

Rest API is full implementation of Spring Entity, JPA Repository, Services , Rest Controller and Security of ATM Simulation Requirement. Since the ATM Simulation Web Front End is implementation of Spring MVC. But there will be no implementation of Repository

Among of those, I have a common library that declare Payload or DTO and model mapper.
