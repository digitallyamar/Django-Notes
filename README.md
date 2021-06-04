# Django-Notes
Notes on my findings on Django

# Use "through" option when using ManyToMany fields that need additional fields
Eg:  visa_not_required = models.ManyToManyField('country.Country', \
        related_name='visa_not_required', through='Visa_Not_Req')

where Visa_Not_Req is another intermediate model.
