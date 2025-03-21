```bash
$> whoami
	0xR19BY
$> cat /root/about_me.rs
```
```rust
#[derive(Debug)]
struct UserProfile {
    code: Vec<&'static str>,
    tools: Vec<&'static str>,
    work: Vec<&'static str>,
    tech_communities: TechCommunities,
    challenge: &'static str,
}

#[derive(Debug)]
struct TechCommunities {
    member: &'static str,
    studying: &'static str,
}

fn main() {
    let user = UserProfile {
        code: vec!["Rust", "Python", "Lua"],
        tools: vec!["SIEM", "SOAR", "WireShark", "Burp Suite", "Arch Linux", "and way more!"],
        work: vec!["L2 Security Analyst", "Threat Hunter", "Detection Engineer"],
        tech_communities: TechCommunities {
            member: "OffSec",
            studying: "Offensive Security Certified Professional",
        },
        challenge: "Currently immersed in the field of webapp pentesting.",
    };

    println!("User Profile: {:?}", user);
}
```
