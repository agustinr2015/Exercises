# Normalization Process
## Step One
### Functional Dependencies:
* PetName - (PetType, PetBreed, PetDOB, OwnerLastName, OwnerFirstName, OwnerPhone, OwnerEmail)
* OwnerEmail - (OwnerFirstName, OwnerLastName, OwnerPhone)
* OwnerPhone - (OwnerFirstName, OwnerLastName, OwnerEmail)
