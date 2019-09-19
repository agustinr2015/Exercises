# Normalization Process
## Step One: Functional Dependencies
* PetName - (PetType, PetBreed, PetDOB, OwnerLastName, OwnerFirstName, OwnerPhone, OwnerEmail)
* OwnerEmail - (OwnerFirstName, OwnerLastName, OwnerPhone)
* OwnerPhone - (OwnerFirstName, OwnerLastName, OwnerEmail)

#### Is every determinant a candidate key?
     Non of the determinants are candidate key.
## Step Two: Break into two reliations
* Owner
* Pet
### Owner:
* 
