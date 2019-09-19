# Normalization Process
## Step One: Functional Dependencies
* PetName - (PetType, PetBreed, PetDOB, OwnerLastName, OwnerFirstName, OwnerPhone, OwnerEmail)
* OwnerEmail - (OwnerFirstName, OwnerLastName, OwnerPhone)
* OwnerPhone - (OwnerFirstName, OwnerLastName, OwnerEmail)

#### Is every determinant a candidate key?
Non of the determinants are Candidate Key.
## Step Two: Break into two relaitions
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
* Pet - (PetName, PetType, PetBreed, PetDOB, OwnerPhone, Service, Date, Charge)
* PetName - PetType, PetBreed, PetDOB, OwnerPhone)

PetName is not a Candidate Key.
## Step Four: Pet and Service Relations:
* Owner - (OwnerPhone, OwnerLastName, OwnerFirstName, OwnerEmail)
* Pet - (PetName, PetBreed, PetType, PetDOB, OwnerEmail)
* Service - (PetName, Service, Charge, Date)
* PetName - (PetType, PetBreed, PetDOB, OwnerPhone)

PetName is a Candidate Key.

Normalization Complete.
## Final Normalization Relations:
* Owner - (OwnerPhone, OwnerLastName, OwnerFirstName, OwnerEmail)
* Pet - (PetName, PetType, PetBreed, PetDOB, OwnerPhone)
* Service - (PetName, Date, Service, Charge)

