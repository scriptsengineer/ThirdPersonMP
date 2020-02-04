# ThirdPersonMP

Tutorial and learn Third Person in Multiplayer
Source Docs: https://docs.unrealengine.com/en-US/Gameplay/Networking/QuickStart/index.html

## Tips and Tricks

### 1 Register another function to impact event.

```C++
//Registering the Projectile Impact function on a Hit event.
SphereComponent->OnComponentHit.AddDynamic(this, &AThirdPersonMPProjectile::OnProjectileImpact);
```

Note: Function need signature
```C++
OnProjectileImpact(UPrimitiveComponent* ,AActor* ,UPrimitiveComponent* , FVector , const FHitResult&)
```
