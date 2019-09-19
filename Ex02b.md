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
## Step three: Owner Functional Dependencies and Candidate Keys.
* OwnerEmail - (OwnerLastName, OwnerFirstName, OwnerPhone)
* OwnerPhone - (OwnerLastName, OwnerFirstName, OwnerEmail)

Both OwnerEmail and OwnerPhone are candidate keys.

Normalization Complete.

Either candidate key can be primary key.
### OwnerPhone as Primary Key:
* Owner - (OwnerPhone, OwnerLastName, OwnerFirstName, OwnerEmail)
* Pet - (PetName, PetType, PetBreed, PetDOB, OwnerPhone)
## Step Four: Pet Functional Dependencies and Candidate Keys.


