```bash
$> whoami
	0xR19BY
$> cat /root/me.txt
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
        code: vec!["Python", "Rust", "Lua"],
        tools: vec!["SIEM", "SOAR", "WireShark", "Burp Suite", "Arch Linux", "and more!"],
        work: vec!["L2 Security Analyst", "Threat Hunter", "Detection Engineer"],
        tech_communities: TechCommunities {
            member: "Hack The Box Academy",
            studying: "Certified Bug Bounty Hunter (CBBH)",
        },
        challenge: "Currently immersed in the field of webapp pentesting.",
    };

    println!("User Profile: {:?}", user);
}
```
